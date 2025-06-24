# Makefile for Serial Program

CC = gcc
CFLAGS = -g -Wall

DEPS =	vars_defs_functions.h timer.h

OBJ = 	serial.o\
	outputWRAT.o

#.SUFFIXES	.c

%.o: %.c $(DEPS)
	$(CC) $(CFLAGS) -c -o $@ $<

serial: $(OBJ)
	$(CC) $(CFLAGS) -o $@ $^ -lm

clean: $(OBJ)
	rm *.o
	rm serial
