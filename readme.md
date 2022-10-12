# Valgrind Exercise
## Standard install via command-line
```
git clone --recursive https://github.com/mahimaarora2208/valgrind
cd <path to repository>
mkdir build
cd build
cmake ..
make
Run tests: ./test/cpp-test
Run program: ./app/shell-app
```

## Run Valgrind 
```
sudo apt install valgrind
cd build
valgrind --leak-check=full -v ./app/shell-app >& ../results/<your file name>.txt
```
## Run KCachegrind
```
sudo apt-get install -y kcachegrind
cd build
valgrind --tool=callgrind  ./app/shell-app
kcachegrind
```
