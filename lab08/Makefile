CC=gcc
CFLAGS_OMP=-std=gnu99 -fopenmp -c -g
LDFLAGS_OMP=-fopenmp

ex1: ex1_test.o ex1.o
	$(CC) $(LDFLAGS_OMP) $^ -o $@

ex1_test.o: ex1_test.c
	$(CC) $(CFLAGS_OMP) $< -o $@

ex1.o: ex1.c ex1.h
	$(CC) $(CFLAGS_OMP) $< -o $@

clean:
	rm -f ex1
	rm -f openmp_example
	rm -f *.o
