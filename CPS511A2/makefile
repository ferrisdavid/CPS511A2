# Windows (cygwin)
ifeq "$(OS)" "Windows_NT"
TARGET = Zeppelin.exe
CFLAGS += -D_WIN32
# OS X/Linux
else
UNAME_S := $(shell uname -s)
	ifeq ($(UNAME_S),Linux)
	TARGET = Zeppelin
	LDFLAGS = -lGL -lGLU -lglut
	CFLAGS = -Wall -std=c99
	endif

	ifeq ($(UNAME_S),Darwin)
	LDFLAGS = -L/opt/homebrew/Cellar/glew/2.2.0_1/lib -L/opt/homebrew/Cellar/freeglut/3.4.0/lib -I/opt/homebrew/include/ -lglew -framework Carbon -framework OpenGL -framework GLUT
	CFLAGS += -D__APPLE__
	TARGET = Zeppelin
	endif
endif


output: surfaceModeller.cpp surfaceModeller.h subdivcurve.h
	g++ surfaceModeller.cpp -o output $(LDFLAGS) ${CFLAGS}

clean:
	rm *.o output
