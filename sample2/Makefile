.PHONY: all

all: start main finish

start:
	@echo "start target"

finish:
	@echo "finish target"

# main$B%?!<%2%C%H$r<B9T$9$k$H(Bmain$B$H$$$&%U%!%$%kL>$N%3%^%s%I$,@8@.$5$l$^$9!#(B
# $@$B$O%?!<%2%C%H$N%U%!%$%kL>!"(B$^$B$OA4$F$NI,?\9`L\$r%9%Z!<%9$G6h@Z$C$?%j%9%H(B
main: *.c myprint.h str.h
	@echo "main target"
	$(CC) $(LDFLAGS) -o $@ $^            

# $<$B$O:G=i$NI,?\9`L\$N%U%!%$%kL>$rI=$7$^$9!#(Bgmake myprint.o$B$H;XDj$7$?$i(B$<$B$O(Bmyprint.c$B$H$J$j$^$9(B
%.o: %.c
	gcc -c $<

.PHONY: clean
clean:
	rm -rf main *.o
