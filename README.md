# C-CPP-Memory-Leak-Detector

This is C/C++ Memory Leak Detector Library. It maintains two databases - Structure Database and Object Database.

User Application registers all its structures with MLD Library at the time of initialization.

Whenever application xcalloc() an object , object record entry is inserted in object database.

If there is any Memory Leak in Application Code, "report_leaked_objects()" function detects that Memory Leak.


### Compilation -
gcc -g -c mld.c -o mld.o

gcc -g -c app.c -o app.o

gcc -g app.o mld.o -o exe

For testing modify app.c file. Create some memory leaks. Do compile as mentioned above. Run the exe file.

./exe
