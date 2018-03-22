all: bin/main.o bin/Hello.o
	g++ -o bin/hello.exe bin/main.o bin/Hello.o

bin/main.o: src/main.cpp 
	g++ -c src/main.cpp -o bin/main.o

bin/Hello.o: src/Hello.cpp
	g++ -c src/Hello.cpp -o bin/Hello.o

clean:
	rm -rf bin/*.exe bin/*.o 

