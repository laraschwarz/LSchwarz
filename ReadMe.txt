Lab #2 ReadMe

1. MainMemory3Test.cct - Final working schematic circuit with all parts. Used for testing.


2. JArcher.clf - The ECC Generator generates five parity bits (P1-P5) from eight data bits (D1-D5), where P5 controls the overall parity of the 13-bit vector. The parity bits are placed at positions 1, 2, 4, 8, and 13. 


3. LSchwarzDataTransmission1.clf - The 13-Bit Data Transmission takes in the data bits and the
parity bits, as well as 13 bits (E1-E13) that allow for specific
data/parity bits to get corrupted.


4. LSchwarzMainMemory5.clf - The Main Memory takes in the possibly corrupted data and parity bits. It then computes C1, C2, C4, C8, and ultimately C to determine whether an error occured during data transmission. To calculate the location of the corrupted bit, the Main Memory uses a 4-16 decoder made up of two 3-8 decoders. Then, the main memory computes P, and then uses the values of  P and C to display error messages, in case bit corruption occurred. If a single-bit error occurs, the Main Memory corrects it.