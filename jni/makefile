CC=g++
SRC=$(wildcard *.c)
OBJS=$(addsuffix .o, $(basename $(SRC)))
CFLAGS=-I$(JAVA_HOME)/include/ -I$(JAVA_HOME)/include/darwin -c
OFLAGS=-Wl --shared
OUT=libhello.dylib

$(OUT):$(OBJS)
	$(CC) $(OFLAGS) -o $@ $<

%.o:%.c
	$(CC) $(CFLAGS) -o $@ $<

