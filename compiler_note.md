gcc **-fsanitize=address** source.c </br>
-> exec </br>
-> return some debug msg </br>

sanitize(殺蟲劑): a tool for check memory bug
> -fsanitize=address: AddressSanitizer; stack, heap, global whether </br> 
> **access out of boundary** (e.g. int a[3]; a[10];) </br>
> **double free** </br>
> **use after return**

> -fsanitize=memory: MemorySanitizer; </br>
> **find uninitialized value**

> -fsanitize=thread: ThreadSanitizer; </br> 
> **find data race** (e.g. multi-thread sync access same value) </br>
> **find deadlock**

-----

gcc **-g** source.c
> **put debug information**, executable file will include source code info.

