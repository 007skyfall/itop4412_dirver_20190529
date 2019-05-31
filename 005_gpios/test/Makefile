src = $(wildcard *.c)
targets = $(patsubst %.c, %, $(src))

CC = gcc
STRIP=strip
CFLAGS = -Wall -g 

all:$(targets)

$(targets):%:%.c
	$(CC) $< -o $@ $(CFLAGS)
	$(STRIP) $@

.PHONY:clean all
clean:
	-rm -rf $(targets) 
