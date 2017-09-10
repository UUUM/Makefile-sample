all: foo

foo: foo.o main.o
	cc -o foo foo.o main.o

foo.o: foo.c
	cc -c -O0 -o foo.o foo.c

main.o: main.c foo.h
	cc -c -O0 -o main.o main.c

clean:
	rm -f foo *.o
