.c.o:   $*.h
	$(CC) $(CFLAGS) -c $*.c

.cpp.o:	$*.h
	$(CC) $(CFLAGS) -c $*.cpp

CC = g++
CFLAGS = -I/usr/local/include/opencv2 -g
LDFLAGS = 	-L/usr/local/lib -lopencv_core \
			-lopencv_highgui -lopencv_imgproc \
			-framework OpenGL -framework GLUT

all:	sinteticTexture simpleTexture 

sinteticTexture:  sinteticTexture.o
	$(CC) $(LDFLAGS) -o $@ $^

simpleTexture:  simpleTexture.o
	$(CC) $(LDFLAGS) -o $@ $^

clean:
	rm *.o *.c~*.*~ sinteticTexture simpleTexture 