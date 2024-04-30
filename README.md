# Multiplexer4to1
# Truth Table
![image](https://github.com/RESMIRNAIR/Multiplexer4to1/assets/154305926/f1dac9e1-e938-4072-bfa9-c17a0a54b7c7)
# Circuit Diagram
![image](https://github.com/RESMIRNAIR/Multiplexer4to1/assets/154305926/f8ea8610-f6fc-4de3-a68a-5a9a4cfcd673)

VERILOG CODE      
`````````````
module m41(y, a, b, c, d, s0, s1);
output y;
input a, b, c, d, s0, s1;
wire w1,w2,w3,w4,w5,w6;
not g1(w1, s0);
not g2(w2, s1);
and g3(w3, a, w1, w2);
and g4(w4, b, s0, w2);
and g5(w5, c, s1, w1), 
and g6(w6, d, s0, s1);
Or g7(y, w3,w4,w5,w6);
endmodule
`````````````

OUTPUT  

![image](https://github.com/YEMANTHKUMAR/Multiplexer4to1/assets/160569469/8bcdbc43-4e8e-474b-b6db-f76994612715)




