# Makefile for netcat

CC=gcc
CFLAGS+= -DMINIX -static -Os

PROGS=nc
SRCS=netcat.c

BINDIR=/usr/bin

MAN=nc.1 netcat.1
SYMLINKS+= $(BINDIR)/$(PROGS) $(BINDIR)/nc


$(PROGS): $(SRCS)
	$(CC) $(CFLAGS) $(SRCS) -o $(PROGS)

install: $(PROGS)
	install -c $(BINDIR)/$(PROGS)
