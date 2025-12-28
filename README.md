# learning / net.c
# Dec 27 2025

# This is a learning project, to shake the rust off and prepare for my next semester, as well as learning/touching on some important topics such as:
 1) Parsing virtual file systems (/proc)
 2) Memory management, "leapfrogging" ,when to use free(), how malloc() works with sizeof() and type casting
 3) Bit manipulation (shifting and masking bits to convert network byte order to human-readable)
 4) Pointer proficiency.
 5) Basic single linked lists.


## Compilation:
I like to use `gcc`:

```bash
gcc -o net.out net.c
```

## Basic usage: 

 ./net.out -a : List all connections regardless of state.
 ./net.out -t : List connections with "ESTABLISHED" state.
 ./net.out -l : List connections with "LISTENING" state.

## To be implemented:

 1) Better connection filtering and search by parsing dynamic command-line args. (optarg or getopt).
 2) Live monitoring of /proc/net/tcp that updates every 2-3 seconds instead of a static capture.
 3) DNS name resolution.
 4) Export to JSON or CSV. 
