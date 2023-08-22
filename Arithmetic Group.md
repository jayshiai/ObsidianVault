
1. ADD B;   A <- A + B
2. ADI 25H;   A <- A + 25H
3. ADD M;   A <- A + M
4. SUB B;   A <- A - B
5. SUM M;
6. SUI 25H;
7. ADC B;   A <- A + B + CF
8. ADC M;
9. ACI 25H;   A <- A + 25H
10. SBB B;   A <- A - B - CF
11. SBB M;
12. SBI 25H;
13. INR B;   B <- B + 1
14. INX B;   BC <- BC + 1
15. INR M;
16. DCR B;
17. DCX B;
18. DCR M;
19. DAD
	1. DAD D;   HL <- HL + DE 
	2. DAD B;   HL <- HL + BC
	3. DAD H;   HL <- HL + HL
20. [[DAA (Decimal Adjust after Addition)]]