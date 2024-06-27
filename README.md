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

### High Level Design
#
![Screenshot (24)](https://github.com/Shokkenn/C-CPP-Memory-Leak-Detector/assets/172527160/3a01bd5b-eeac-442f-8d3c-249a0d3bc4ea)
#
![Screenshot (27)](https://github.com/Shokkenn/C-CPP-Memory-Leak-Detector/assets/172527160/e9007f8c-788a-4683-9ab4-c1f1fd451d0d)
#
![Screenshot (23)](https://github.com/Shokkenn/C-CPP-Memory-Leak-Detector/assets/172527160/468e8076-f8f1-4be0-954a-9853dca43748)

### Testing MLD Library
#
![Screenshot (28)](https://github.com/Shokkenn/C-CPP-Memory-Leak-Detector/assets/172527160/843006d7-ca52-47bc-88b1-521c763d2d84)
![Screenshot (29)](https://github.com/Shokkenn/C-CPP-Memory-Leak-Detector/assets/172527160/fd128203-fc4e-4554-bcc0-e9228d4297af)
![Screenshot (30)](https://github.com/Shokkenn/C-CPP-Memory-Leak-Detector/assets/172527160/878f9188-1b7e-41cd-8d76-ca5560b0d33d)
![Screenshot (31)](https://github.com/Shokkenn/C-CPP-Memory-Leak-Detector/assets/172527160/9c8c8f25-9450-4e49-896e-0ca015ae76ed)
