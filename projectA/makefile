sub.o:./src/other1.c
	gcc -c ./src/other1.c -I include -o sub.o
	mv sub.o ./lib
add.o:./src/other2.c
	gcc -c ./src/other2.c -I include -o add.o
	mv add.o ./lib
libcal.a:
	ar rcs libcal.a ./lib/*.o
	mv lincal.a ./lib
main:
	gcc -o main test.c -Llib/  -lcal -I include
clean:
	rm ./lib/*.o;rm main

