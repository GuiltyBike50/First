# Усложненный make-file.  Введены переменные для параметров компиляции и исполняемых файлов

.PHONY: all debug release clean

RELEASE_FLAGS = -O2 -Wall -DNDEBUG
DEBUG_FLAGS   = -g -O0 -Wall
RELEASE_EXEC  = Kazino_Royal
DEBUG_EXEC    = Kazino_Royal-dbg
SOURCE        = Kazino_Royal.cpp

all: debug release

debug: $(DEBUG_EXEC)

Kazino_Royal-dbg: $(SOURCE)
	g++ $(DEBUG_FLAGS) $(SOURCE) -o $(DEBUG_EXEC) 

release: $(RELEASE_EXEC)

Kazino_Royal: $(SOURCE)
	g++ $(RELEASE_FLAGS) $(SOURCE) -o $(RELEASE_EXEC)

clean:
	rm -f $(RELEASE_EXEC) $(DEBUG_EXEC)

