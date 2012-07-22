# Makefile for netcat
PROGS=netcat
SRCS=netcat.c

BINDIR=/usr/bin

MAN=nc.1 netcat.1
SYMLINKS+= $(BINDIR)/$(PROGS) $(BINDIR)/nc

CPPFLAGS+= -DMINIX -DGAPING_SECURITY_HOLE -static

.include <bsd.prog.mk>
