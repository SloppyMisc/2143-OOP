# ============================
# Windows MinGW Makefile
# ============================

CXX := g++
CXXFLAGS := -Wall -std=c++17
TARGET := $(notdir $(CURDIR))
SRC := main.cpp
INCLUDES := -I./includes

all: $(TARGET).exe

$(TARGET).exe: $(SRC)
	$(CXX) $(CXXFLAGS) $(INCLUDES) -o $@ $^

run: $(TARGET).exe
	./$(TARGET).exe

clean:
	del /f $(TARGET).exe

.PHONY: all run clean
