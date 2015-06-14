# 偽りのターゲットPHONY   allというファイルが存在していても気にしない
.PHONY: all

# デフォルトターゲットとしての指定
all: main

# mainターゲットを実行するにはmain.oターゲットが最新+str.hが最新となっていること
main: main.o str.h
	gcc -o main main.o

main.o: main.c
	gcc -c main.c

.PHONY: clean
clean:
	rm -rf main main.o
