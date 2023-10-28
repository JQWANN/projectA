in=include
sub.o:./src/other1.c
	gcc -c $^ -I in -o $@
	mv $@ lib
add.o:./src/other2.c
	gcc -c $^ -I in -o $@
	mv $@ lib
libcal.a:
	ar rcs $@ lib/*.o
	mv $@ lib
main:
	gcc -o $@ test.c -Llib  -lcal -I in
clean:
	rm lib/*.o;rm main

