CC = gcc
DEBUG = -g
CFLAGS = -Wall -lpthread -c $(DEBUG)
LFLAGS = -Wall -lpthread $(DEBUG)

main: main.o mqtt.o
	$(CC) $(LFLAGS) main.o mqtt.o -o main

main.o: main.c mqtt.h
	$(CC) $(CFLAGS) main.c

mqtt.o: mqtt.h mqtt.c
	$(CC) $(CFLAGS) mqtt.c

clean:
	rm -rf *.o *~ main
