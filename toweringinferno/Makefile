CXXFLAGS := -I ../libtcod-1.5.0/include -std=c++0x -Wall
%o: %.cpp
	$(CXX)  $(CXXFLAGS) -c $<


toweringinferno: game.o world.o main.o proceduralgeneration/floorgenerator.o player.o heatvision/heatvisionsystem.o
	$(CXX) $^ -o toweringinferno -ltcodxx -ltcod -ltcodgui -L../libtcod-1.5.0

clean:
	rm -f *.o toweringinferno

all: toweringinferno
