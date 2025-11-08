# =========================================================
# SDL2 Example Makefile (VS Code + MinGW64)
# =========================================================

CXX := g++
CXXFLAGS := -Wall -std=c++17 -IC:/msys64/mingw64/include/SDL2
LDFLAGS := -LC:/msys64/mingw64/lib -lmingw32 -lSDL2main -lSDL2

TARGET := program00
SRC := main.cpp

all: $(TARGET)

$(TARGET): $(SRC)
	$(CXX) $(CXXFLAGS) -o $@ $^ $(LDFLAGS)

run: $(TARGET)
	./$(TARGET)

clean:
	del $(TARGET).exe

.PHONY: all run clean
