foo: main.o greeter.o
	gcc -o foo main.o greeter.o

main.o: main.c
	gcc -c -Wall -Wextra -Werror -o main.o main.c

greeter.o: greeter.c
	gcc -c -Wall -Wextra -Werror -o greeter.o greeter.c
