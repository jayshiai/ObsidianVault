#2ndYear #microprocessor 


# Stack

## Push
- SP increaments. Data Added.
- Push always works with 16 bit data. i.e. for it to work you have to use register pair. Can't use single register.
- Lower address(in number not height) goes into  lower byte address
## Pop
- Data removed. SP decreament.
- 16 bit data used.

### Register A and Stack
- Since stack works with 16 bit data, and A register doesn't have any pair, a new instruction `PSW` is used which pairs A with F (flag register) . F is the lower byte address

# I/O

## IN and OUT
- I/O devices have 8-bit addresses (compared to 16 bit addresses of memory).
- `IN 40H` means data from I/O device at address at 40H in inputed into Register A. Same with output.

# Machine Control
- SIM
- RIM
- DI (Disable Interrrupt)
- EI (Enable Interrupt)
- NOP (No Operations)
- HLT (Halt)