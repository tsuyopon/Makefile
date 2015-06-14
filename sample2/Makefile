.PHONY: all

all: start main finish

start:
	@echo "start target"

finish:
	@echo "finish target"

# mainターゲットを実行するとmainというファイル名のコマンドが生成されます。
# $@はターゲットのファイル名、$^は全ての必須項目をスペースで区切ったリスト
main: *.c myprint.h str.h
	@echo "main target"
	$(CC) $(LDFLAGS) -o $@ $^            

# $<は最初の必須項目のファイル名を表します。gmake myprint.oと指定したら$<はmyprint.cとなります
%.o: %.c
	gcc -c $<

.PHONY: clean
clean:
	rm -rf main *.o
