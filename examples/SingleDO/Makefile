CC=gcc
CCFLAGS= -g -Wall -I../../include -I../ParseParams
LDFLAGS= -lpowerdaq32

target= SingleDO
OBJECTS= SingleDO.o ../ParseParams/ParseParams.o

all: $(target)

$(target): $(OBJECTS) 
	$(CC) $(OBJECTS) $(LDFLAGS) -o $@ 

%.o: %.c
	$(CC) $(CCFLAGS) -c $< -o $@

clean:
	rm -f $(OBJECTS)
	rm -f $(target)
