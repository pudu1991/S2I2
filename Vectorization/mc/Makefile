
TARGETS = exptest mc0 mc1 mc2 mc3 mc4 mc5

CXX = icpc
CXXFLAGS = -xHOST -O3 -ipo -no-prec-div  -vec-report6 -mkl=sequential

all:	$(TARGETS)

%.o : %.cc timerstuff.h
	$(CXX) -c $(CFLAGS) $(CPPFLAGS) $< -o $@

clean:
	/bin/rm -f *.o $(TARGETS) core* *~
