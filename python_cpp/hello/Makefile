all:
	swig -python example.i
	gcc -c example.c example_wrap.c -I/usr/include/python2.7
	ld -shared example.o example_wrap.o -o _example.so

clean:
	rm -f example_wrap.c example_wrap.o _example.so
	rm -f example.pyc example.o example.py
