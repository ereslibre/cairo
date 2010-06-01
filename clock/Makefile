all: clock.o main.o
	g++ -o clock `pkg-config --libs cairo gtkmm-2.4` clock.o main.o

clock.o: clock.cc clock.h
	g++ -c `pkg-config --cflags cairo gtkmm-2.4` clock.cc

main.o: main.cc
	g++ -c `pkg-config --cflags cairo gtkmm-2.4` main.cc

clean:
	rm *.o clock
