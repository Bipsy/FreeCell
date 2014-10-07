CC = gcc
CFLAGS = -Wall -g
INCDIR = ../include
INCLUDES = -I$(INCDIR)
LFLAGS = -L../lib
SRCDIR = ../src
SRCS = $(SRCDIR)freecell.c $(SRCDIR)lookup3.c $(SRCDIR)score_strategies.c $(SRCDIR)stateHashTable.c $(SRCDIR)state_functions.c
OBJS = $(SRCS:.c=.o)
EXE = FreeCell

all: $(EXE)
     
$(EXE): $(OBJS)
        $(CC) $(CFLAGS) $(INCLUDES) -o $(EXE) $(OBJS) $(LFLAGS) $(LIBS)

.c.o: 
      $(CC) $(CFLAGS) $(INCLUDES) -c $< -o $@

clean: 
        $(RM) *.o *~ $(EXE)
