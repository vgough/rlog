**NOTE: This library is no longer being maintained.**   In 2003, RLog provided functionality that was not commonly available, but there are a number of good logging libraries available today.


RLog provides a flexible message logging facility for C++ programs and libraries. It is subscription based, meaning you can subscribe to messages of your choice in an number of ways: by hierarchical channel name (e.g. "debug", "debug/special", "error", etc.), or filename, component name, etc.

Log messages are individually enabled. It is meant to be fast enough to leave in production code - even where it may be called many times, as both the GCC and Intel compilers reduce the logging overhead a couple clock cycles if they are dormant (with no subscribers).

RLog was originally the internal logging mechanism of [EncFS](http://www.arg0.net/encfs), but was eventually broken out into a separate project.  It has been tested on a wide variety of systems - see the homepage for details.

Homepage: http://www.arg0.net/rlog