CC = gcc
CFLAGS = -pthread

SRC = server.c
OBJ = $(SRC:.c=.o)
EXECUTABLE = server

all: $(EXECUTABLE)

$(EXECUTABLE): $(OBJ)
	$(CC) $(OBJ) -o $(EXECUTABLE) $(CFLAGS)

%.o: %.c
	$(CC) -c $< -o $@ $(CFLAGS)

clean:
	rm -f $(OBJ) $(EXECUTABLE)
