Compilation steps

g++ -I $JAVA_HOME/include -I $JAVA_HOME/include/darwin -c lpsolve5j.cpp 
g++ -dynamiclib lpsolve5j.o -compatibility_version 5.5.0 -current_version 5.5.0 -o liblpsolve55j.dylib -Wl,-install_name,/usr/local/lib/liblpsolve55j.dylib -llpsolve55
sudo cp liblpsolve55j.dylib /usr/local/lib
