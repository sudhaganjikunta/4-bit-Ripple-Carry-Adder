## 4-bit-Ripple-Carry-Adder
A ripple carry adder is a simple method to build a multi-bit binary adder by chaining together 1-bit full adders. In this architecture, the carry output of each bit’s addition “ripples” (propagates) to the next higher bit as its carry input.A 4-bit ripple carry adder takes two 4-bit binary numbers, A=A3 A2 A1 A0 and B=B3 B2 B1 B0 ,carry-in Cin  and produces a 4-bit sum S=S3 S2 S1 S0 and final carry out Cout.

-----
## Structure & Operation
* The 4-bit RCA is made by cascading 4 full adders.
* The least significant bit (LSB) full adder adds A0,B0,Cin and producing S0 and C1.
* Then the next bit’s full adder uses inputs A1,B1 and C1,producing s1&c2.
* This continues until the most significant bit (MSB) adder, which outputs S3 and Cout.
* Thus the carry “ripples” from the LSB stage to the MSB stage.

   |A0  B0  Cin → FA → S0, C1|
   |A1  B1  C1  → FA → S1, C2|
   |A2  B2  C2  → FA → S2, C3|
   |A3  B3  C3  → FA → S3, Cout|
-----
## Advantages
* Simplicity — The design is straightforward and easy to understand.
* Low hardware overhead — It uses minimal extra logic beyond the full adders.
* Modular / Scalable — You can build an n-bit adder by chaining n full adders.
## Disadvantages
* One of the main drawbacks of a ripple carry adder is propagation delay.Each full adder stage has some delay before its sum and carry outputs are stable after its inputs are applied.
* Not ideal for high-speed circuits — For high-frequency designs, more advanced adders are used.
  
