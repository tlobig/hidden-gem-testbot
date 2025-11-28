CXX = g++
CXXFLAGS = -std=gnu++20 -O2 -pipe -Wall --pedantic -flinker-output=exec --static
# CXXFLAGS = -std=gnu++20 -O2 -pipe

ifeq ($(OS),Windows_NT)
    TARGET = bot.exe
    RM = del /Q
else
    TARGET = bot
    RM = rm -f
endif

SRC = bot.cpp

$(TARGET): $(SRC)
	$(CXX) $(CXXFLAGS) -o $(TARGET) $(SRC)

clean:
	$(RM) $(TARGET)

