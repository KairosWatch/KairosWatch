CFLAGS = -g -Wall -I../../../csrc/.  `sdl2-config --cflags`

SRC = $(shell ls ../../../csrc/*.c) $(shell ls ../common/*.c ) main.c menu.c gui.c datecalc.c

OBJ = $(SRC:.c=.o)

helloworld: $(OBJ) 
	$(CC) $(CFLAGS) $(LDFLAGS) $(OBJ) `sdl2-config --libs` -o u8g2_sdl

clean:	
	-rm $(OBJ) u8g2_sdl

