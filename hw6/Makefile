BINDIR = build

all: $(BINDIR)/test_particle $(BINDIR)/test_event

$(BINDIR)/test_particle : test_particle.cpp particle.cpp vectors.cpp uniqueid.cpp
	clang++ -std=c++11 -stdlib=libc++ $^ -o $@ 

$(BINDIR)/test_event : test_event.cpp event.cpp particle.cpp vectors.cpp uniqueid.cpp
	clang++ -std=c++11 -stdlib=libc++ $^ -o $@ 

# may need to add -Weverything flag or similar at some point

clean:
	rm $(BINDIR)/*