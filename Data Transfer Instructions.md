#studynotes #microprocessor

1. MVI B, 25H;   B <- 25H
2. LXI B, 2000H;   BC <- 2000H
3. MVI M, 25H;   M <- 25H. M is location stored in HL pair.
4. MOV B, C;   B <- C
5. LDA 2000H;   A <- [2000H]
6. STA 3000H;   A -> [3000H]
7. LHLD 5000H;   L <- [5000H] H <- [5001H]
8. SHLD 5000H;   L -> [5000H] H -> [5001H]
9. LDAX B;   A <- [BC]
10. STAX D;   A -> [DE]
11. PCHL ;   PC <- HL
12. SPHL ;   SP <- HL
13. XCHG ;   HL <--> DE
14. XTHL ;   L <--> [SP]  H <--> [SP+1]