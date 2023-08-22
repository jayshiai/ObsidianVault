#cso
It has two steps :
	- Fetch
	- Execute

![[Pasted image 20230822200102.png]]

## Fetch Cycle

1. Program Counter (PC) holds address of next instruction to fetch
2. Processor fetchers instruction
3. Increment PC
4. Instruction loaded in IR (Instruction Register)
5. Interpretation of instruction and performing action.

## Execute cycle

1. Data transfer between Processor and Memory
2. Data transfer between Processor and I/O
3. Data Processing : Some arithmetic or logical operation on data.
4. Control : Alteration of sequence of operations, eg. Jump

## Example of Program Execution

![[Pasted image 20230822200808.png]]


# Instruction Cycle State Diagram

![[Pasted image 20230822201438.png]]


However above Instruction cycle can be changed with [[Interrupts]]