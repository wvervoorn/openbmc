# Copyright 2015-present Facebook. All Rights Reserved.
lib: libsdr.so

libsdr.so: sdr.c
	$(CC) $(CFLAGS) -fPIC -c -o sdr.o sdr.c
	$(CC) -lm -shared -o libsdr.so sdr.o -lc

.PHONY: clean

clean:
	rm -rf *.o libsdr.so
