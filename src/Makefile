# Makefile to compile rudisvg
# using g++

PP=g++ -std=c++11

#CFLAGS
EXTRAS= # e.g add EXTRAS=-DDEBUG for debug mode
RUDISVGLINKFLAGS = -I/usr/X11R6/include -I/usr/X11R6/include/X11 -L/usr/X11R6/lib -L/usr/X11R6/lib/X11 -lX11 #-lX11
RUDISVG = rudisvg
RUDISVGCPP = rudisvg.cpp
PUGIXML = pugixml/pugixml.cpp
ORUDISVG = rudisvg.o pugixml.o

all: $(RUDISVG)

rudisvg: $(ORUDISVG)
	$(PP) -o rudisvg $(ORUDISVG) $(RUDISVGLINKFLAGS)

rudisvg.o: $(RUDISVGCPP)
	$(PP) -c $(RUDISVGCPP) $(EXTRAS)

pugixml.o: $(PUGIXML)
	$(PP) -c $(PUGIXML) $(EXTRAS)

clean:
	$(RM) $(RUDISVG) *.o
