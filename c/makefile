CC = gcc

TARGET = demo

IFLAGS = -Iinc

SRC_FILES = $(wildcard src/*.c)

OBJS = $(patsubst %.c, %.o, $(SRC_FILES))

CFLAGS = -g

all : $(TARGET)

$(OBJS) : %.o: %.c
	$(CC) -c $< -o $@ $(IFLAGS) $(CFLAGS)

$(TARGET):$(OBJS)
	$(CC) -o $(TARGET) $(OBJS)