NAME := foo
OBJFILES := obj/main.o obj/greeter.o
LDFLAGS ?=
CFLAGS ?= -Wall -Wextra -Werror

$(NAME): $(OBJFILES)
	$(CC) $(LDFLAGS) -o $@ $^

obj/%.o: src/%.c
	$(CC) -c $(CFLAGS) -o $@ $^
