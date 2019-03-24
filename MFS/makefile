all:init_disk MFS
init_disk: init_disk.o
	gcc init_disk.o -o init_disk
MFS: MFS.o
	gcc MFS.o -o MFS -Wall -D_FILE_OFFSET_BITS=64 -g -pthread -lfuse3 -lrt -ldl

MFS.o: MFS.c
	gcc -Wall -D_FILE_OFFSET_BITS=64 -g -c -o MFS.o MFS.c
init_disk.o: init_disk.c
	gcc -Wall -D_FILE_OFFSET_BITS=64 -g -c -o init_disk.o init_disk.c
.PHONY : all
clean :
	rm -f MFS init_disk MFS.o init_disk.o
