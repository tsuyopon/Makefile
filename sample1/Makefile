# $B56$j$N%?!<%2%C%H(BPHONY   all$B$H$$$&%U%!%$%k$,B8:_$7$F$$$F$b5$$K$7$J$$(B
.PHONY: all

# $B%G%U%)%k%H%?!<%2%C%H$H$7$F$N;XDj(B
all: main

# main$B%?!<%2%C%H$r<B9T$9$k$K$O(Bmain.o$B%?!<%2%C%H$,:G?7(B+str.h$B$,:G?7$H$J$C$F$$$k$3$H(B
main: main.o str.h
	gcc -o main main.o

main.o: main.c
	gcc -c main.c

# target$B$r(Btarget1$B$H;XDj$7$F$b!"(Btarget2$B$H;XDj$7$F$b<B9T$5$l$k(B
target1 target2: main.o str.h
	@echo "target1 or target2 executed"    # $B@hF,$K(B@$BIUM?$G=PNOM^@)(B
	-hogehoge                              # $B@hF,$K(B-$BIUM?$G%(%i!<$rL5;k(B
	@echo "finished"

.PHONY: clean
clean:
	rm -rf main main.o
