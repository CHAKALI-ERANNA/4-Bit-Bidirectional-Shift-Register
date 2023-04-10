# 4-Bit-Bidirectional-Shift-Register
  Hello everyone! we designed and verified the PISO shift register in our previous post, Here I'm with 4-bit Bi-directional Shift Register (seems similar to PISO if you understand that it would be easy).

Lets learn together.



📌By this bidirectional shift register data can be shifted either from left to right or right to left(name itself justifies this).



📌 Operation : When right_Lleft is HIGH, this control signal allows the data to shift from left to right.



📌Similarly when right_Lleft control signal becomes LOW it allows data to shift from right to left.



📌In addition to the circuit diagram shown in the figure I just added the reset pin too, so when reset pin gets activated(active low) the register will be cleared.



📌Circuit Diagram : Observe the circuit diagram when RIGHT/LEFTbar signal is HIGH G1 to G4 gates are enabled so the state of the Q output passed to the D input of the following flip flop.



📌Lets make it way more clear Observe the G2 gate if RIGHT/LEFTbar is HIGH the G6 gets one of its input as 0(low) so G6 gate output is 0 (AND gate) G2 gates gets one of its input as 1(high) so whatever the other input that is the output of G2, so output of (first) previous FF is passed to the following FF.



📌So in this way the data is shifted from left to right.



📌When RIGHT/LEFTbar is LOW gates G5 through G8 are enabled, Q output of each flip-flop is passed through to the D input of the preceding flip-flop. So the data is shifted from right to left.


