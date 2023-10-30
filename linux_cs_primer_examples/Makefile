CC=gcc
CFLAGS=-Wall -ansi -pedantic-errors -g
OBJECTS=my_prog.o lib1.o lib2.o
HEADERS=lib1.h lib2.h

all: my_prog

lib1.o: lib1.c $(HEADERS)
lib2.o: lib2.c $(HEADERS)
my_prog.o: my_prog.c $(HEADERS)
my_prog: $(OBJECTS)

clean:
	rm -f my_prog $(OBJECTS)

run: my_prog
	./my_prog

# It's a good idea to add targets like 'test', for example, to test your
# application against known input & output files...
