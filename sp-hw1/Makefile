CC := gcc
CFLAGS := -O2 -Wall

READ := -D READ_SERVER
WRITE := -D WRITE_SERVER

INPUT := server.c

OUTPUT_READ := read_server
OUTPUT_WRITE := write_server

.PHONY: all read write clean

all: read write

read: server.c
	$(CC) $(CFLAGS) $(INPUT) $(READ) -o $(OUTPUT_READ)

write: server.c
	$(CC) $(CFLAGS) $(INPUT) $(WRITE) -o $(OUTPUT_WRITE)

clean:
	rm -f $(OUTPUT_READ)
	rm -f $(OUTPUT_WRITE)

#./read_server 3333 ; ./write_server 3334
