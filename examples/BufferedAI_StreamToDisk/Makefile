CC=gcc
CCFLAGS= -g -Wall -I../../include -I../gnuplot -I../ParseParams -I../ReadStreamFile
LDFLAGS= -lpowerdaq32 -lpthread

target= BufferedAI_StreamToDisk
OBJECTS= BufferedAI_StreamToDisk.o ../gnuplot/gnuplot.o ../ParseParams/ParseParams.o

all: $(target)

$(target): $(OBJECTS) 
	$(CC) $(OBJECTS) $(LDFLAGS) -o $@ 

%.o: %.c
	$(CC) $(CCFLAGS) -c $< -o $@

clean:
	rm -f $(OBJECTS)
	rm -f $(target)
