# Makefile for BME280 project

CC = gcc
CFLAGS = -Wall -I. -lrt

SRC = capteur.c bme280.c
OBJ = $(SRC:.c=.o)
EXECUTABLE = bme280

all: $(EXECUTABLE)

$(EXECUTABLE): $(OBJ)
	$(CC) $(OBJ) -o $(EXECUTABLE) $(CFLAGS)

%.o: %.c
	$(CC) -c $< -o $@ $(CFLAGS)

clean:
	rm -f $(OBJ) $(EXECUTABLE)
