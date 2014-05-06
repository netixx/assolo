assolo
======

This fork is almost identical to the original Assolo project.

Assolo is a tool for measuring bandwidth based on the pathChirp tool.


The intent of this project is to fix bugs in the original impelemntation.

Bugs fixed :

* When all options are set on the master node, the receiver nodes crashes
  * Fixed by increasing the number of bytes in write on the master node to strlen(data) instead of 100
  * Fixed on receiver by increasing array of parameter to 50 instead of 20
