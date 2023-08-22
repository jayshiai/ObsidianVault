1. AND
	1. ANA B;   A <- A ^ B
	2. ANA M;
	3. ANI 25H;
2. OR
	1. ORA B;
	2. ORA M;
	3. ORI 25H;
3. XOR
	1. XRA B;
	2. XRA M;
	3. XRI 25H;
4. Rotates
	1. RLC ;   Number in A in rotated. And MSB (left [L] most digit) is stored in CF
	2. RRC ;   Number in A in rotated. And LSB (right [R] most digit) is stored in CF
	3. RAL ;   Number in A along with CF is rotated with CF in front of MSB. i.e CF becomes LSB
	4. RAR ;   Number in A along with CF is rotated with CF in front of LSB. i.e CF becomes MSB
5. Compare
	1. CMP B;   A - B -> ZF/CF
	2. CPI 25H;
	3. CMP M;
6. STC ;   CF <- 1
7. CMC ;   CF <- !(CF)
8. CMA ;   A <- !(A)