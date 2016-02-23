CC = gcc

.PHONY: clean

testapp: ../src/libsonicvox.a
	$(CC) test_app.c -o test_app -I../include ../src/libsonicvox.a -lm
       
clean:
	-rm $(OBJS) test_app

%.o: %.c
	$(CC) -c -Wall -O2 -o $@ -I include $<
	