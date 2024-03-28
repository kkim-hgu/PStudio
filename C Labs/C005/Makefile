#CC = clang
CC = gcc
CFLAGS = -W -Wall
TARGETS = C005
OBJS = main.c

all : $(TARGETS)

debug : $(TARGETS)
debug : OPTION = -DDEBUG_MODE

$(TARGETS) : $(OBJS)
	$(CC) $(CFLAGS) $(OPTION) -o $@ $^

%.o : %.c %.h
	$(CC) -c $(CFLAGS) $(OPTION) $< -o $@

clean :
	rm *.o C005
