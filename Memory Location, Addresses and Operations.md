Memory is made up of millions of storage cells, each of which stores 1 bit.
Data is usually accessed in n-bit groups. n is called word length.

- a k-bit address has $2^k$ memory locations.
- 24-bit memory has $2^{24} = 16M$
- 32-bit memory has $2^{32} = 4G$
- $1T = 2^{40}$

- Byte locations are 0,1,2 and in 32-bit memory successive word locations are 0,4,8.. (since 4 bytes = 1 word in 32-bit)

# Big Endian and Little Endian

- Big endian : Lower byte addresses are used for the most significant bytes of word.
- Little endian: Lower byte addresses are used for least sign