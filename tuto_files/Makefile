NAME := foo
OBJFILES := $(addprefix obj/, main.o greeter.o)
LDFLAGS ?=
CFLAGS ?= -Wall -Wextra -Werror

$(NAME): $(OBJFILES)
	$(CC) $(LDFLAGS) -o $@ $^

obj/%.o: src/%.c
	@mkdir -p $(dir $@)
	$(CC) -c $(CFLAGS) -o $@ $^

clean:
	rm -rf $(NAME) $(OBJFILES)

.PHONY: clean
