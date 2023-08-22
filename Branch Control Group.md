#microprocessor #studynotes 

1000 JMP 2000H;   Will go to 2000 address. ie. PC = 2000H

*Conditional Jumps*
1. JC ;  Jump if CF =1
2. JNC ;   Jump if CF = 0
3. JZ ;   Jump if ZF = 1, ie. result = 0
4. JNZ ;
5. JPE ;   PF = 1 (parity even)
6. JPO;   PF = 0 (parity odd)
7. JM ;   SF = 1
8. JP ;   SF = 0

*Looping*
1. Use Jump

*Call*
```
1000 CALL 2000H;
1003 ...
.
.
.
2000 ...
.
2005 RET;   Returns 1003 (since 1001 has 00 and 1002 has 20 from 2000H)
```

*RST-n*
RST 0;    Calls 0000
RST 1;    Calls 0008
RST 2;    Calls 0010
RST 3;    Calls 0018
RST 4;    Calls 0020
RST 5;    Calls 0028
RST 6;    Calls 0030
RST 7;    Calls 0038

