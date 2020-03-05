CC = gcc
WFLAGS = -Wall -Wextra
EXE = 537ps

$(EXE):	stats.o processList.o options.o
	$(CC) $(WFLAGS) -o $(EXE) stats.o processList.o options.o

options.o:	options.c processList.h stats.h
	$(CC) $(WFLAGS) -c options.c

processList.o:	processList.c processList.h
	$(CC) $(WFLAGS) -c processList.c

stats.o:	stats.c stats.h
	$(CC) $(WFLAGS) -c stats.c

clean:
	rm -r $(EXE) *.o

recompile:	clean $(EXE)

