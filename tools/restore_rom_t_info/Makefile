
CC=gcc
#CFLAGS += -DTRENDCHIP
OBJS=restore_rom_t_info.o
EXECS=restore_rom_t_info
all: restore_rom_t_info

.c.o:
	$(CC) -c $<

restore_rom_t_info: $(OBJS) 
	$(CC) -o $@ $(OBJS)

clean:
	rm -f *.o *.a $(EXECS)

.PHONY : release
release:
	rm -rf *.c
	mv Makefile.release Makefile
