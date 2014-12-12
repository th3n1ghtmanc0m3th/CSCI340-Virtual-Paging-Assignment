CSCI340 Virtual Paging Assignment
==================================

CSCI340 (Operating Systems)  
California State University, Chico  
Public Code

Slight additions   
By Bryan Dixon - 2014

Adopted from assignment  
By Andy Sayler - 2012  
http://www.andysayler.com

That was adopted from  
assignment by Dr. Alva Couch  
http://www.cs.tufts.edu/~couch/

With help from:  
Junho Ahn - 2012

Folders
=================================
-  handout - Assignment description and documentation

Files
=================================
-  Makefile - GNU makefile to build all relevant code
-  pager-basic.c - Basic paging strategy implementation that runs one process at a time.  
-  pager-lru.c - LRU paging strategy implementation (you code this).
-  pager-predict.c - Predictive paging strategy implementation (you code this).
-  api-test.c - A pageit() implmentation that tests that simulator state changes
-  simulator.c - Core simualtor code (look but don't touch)
-  simulator.h - Exported functions and structs for use with simulator
-  programs.c - Defines test "programs" for simulator to run
-  pgm*.pseudo - Pseudo code of test programs from which programs.c was generated.

Executables
=================================
-  test-* - Runs simulator using "programs" defined in programs.c and paging strategy defined in pager-*.c. Includes various run-time options. Run with '-help' for details.
-  test-api - Runs a test of the simulator state changes

Examples
=================================
Build:
```bash
$ make
```

Clean:
```bash
$ make clean
```
View test options:
```bash
$ ./test-* -help
```
Run pager-basic test:
```bash
$ ./test-basic
```
Run API test:
```bash
$ ./test-api
```
