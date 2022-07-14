CC = g++
CPPFLAGS = -c -Wall
OBJ = obj/
SRC = src/
BIN = bin/
INCLUDE = inc/

all: app

app:$(OBJ)file1.o
	$(CC) -o app $(OBJ)file1.o 
	mv app $(BIN) 

$(OBJ)file1.o: $(SRC)file1.cpp
	$(CC) $(CPPFLAGS) $(SRC)file1.cpp -I $(INCLUDE)
	mv file1.o $(OBJ)

clean:
	rm -f a.out app *.o
	rm -f $(OBJ)*.o
	rm -f $(BIN)app
