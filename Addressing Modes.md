
1. Immediate :- Data is given in instruction
	1. MVI B, 25H;   MVI = Move immediately. B <- 25H.
	2. LXI B, 2000H;   LXI = Load Immediately. BC <- 20 (B) 00 (C) 
2. Register :- Data in register
	1. MOV B, C;   B <- C
	2. INR B;    B <- B + 1
	3. INX B;   BC <- BC + 1
3. Direct :- Address in instruction.
	1. LDA 2000H;   A <- [2000H]
	2. STA 3000H;   A -> [3000H]
4. Indirect :- Address in register
	1. LDAX B;   A <- [BC]
	2. STAX D;   A -> [DE]
5. Implied
	1. STC ;   CF <- 1
	2. CMC ;   CF <- !(CF)