# 偽りのターゲットPHONY   allというファイルが存在していても気にしない
.PHONY: all

# デフォルトターゲットとしての指定
all: main

# mainターゲットを実行するにはmain.oターゲットが最新+str.hが最新となっていること
main: main.o str.h
	gcc -o main main.o

main.o: main.c
	gcc -c main.c

# targetをtarget1と指定しても、target2と指定しても実行される
target1 target2: main.o str.h
	@echo "target1 or target2 executed"    # 先頭に@付与で出力抑制
	-hogehoge                              # 先頭に-付与でエラーを無視
	@echo "finished"

.PHONY: clean
clean:
	rm -rf main main.o
