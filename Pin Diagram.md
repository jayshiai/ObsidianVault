![[Pasted image 20230830112543.png]]

ResetIN - Resets
ResetOut- Send reset signal to other devices
Ready - I/O devices inform processor they are ready
RD - 1 if not read. 0 if processor wants to read.
WR - 1 if not write. 0 if processor wants to write.
S1 - Action performed was an input
S0 - Action performed was an output
IO/m - informs where the action was performed
VCC / GND - common sense
A15 - A8 - Only address bus
AD7 - AD0 - Address as well as data bus
ALE - Address Latch Enable

S1D - Serial Input
S0D - Serial Output

Trap, RST, INTR - Interrupts with Trap top prior and INTR lowers prior
INTA - Informs that interrupt will be processed
HOLD - DMA ( Direct memory access)
HLDA - DMA granted