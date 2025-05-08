### ENCODER 8TO3 DATAFLOW Modelling

## Developed by: K.Preetha
## Register Number: 212224100044

**AIM:**

To implement  Encoder 8 To 3 in Dataflow Modelling using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:** Quartus prime

**THEORY**

**Encoder 8 To 3**

The 8 to 3 line Encoder is also known as Octal to Binary Encoder. In 8 to 3 line encoder, there is a total of eight inputs, i.e., D0, D1, D2, D3, D4, D5, D6, and D7 and three outputs, i.e., A0, A1, and A2. In 8-input lines, one input-line is set to true at a time to get the respective binary code in the output side. Below are the block diagram and the truth table of the 8 to 3 line encoder.

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/0bc242c1-eb9e-4c47-afe5-30428470efc3)

Figure 01  Block Diagram of Encoder 8 * 3

**Truth Table**

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/35496b14-ae6e-4cd1-9abd-d6736b576575)

The logical expression of the term A0, A1, and A2 are as follows:

A0 = D1 + D3 + D5 + D7

A1 = D2 + D3 + D6 + D7

A2 = D4 + D5 + D6 + D7

Logical circuit of the above expressions is given below:

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/95acaee6-c873-4c75-89eb-ef09fb158053)

Figure 02  Encoder 8 * 3

**Procedure**
```
1.Define the module and its ports
2.Analyzing the Logic
3.Write the dataflow modeling equations
4.Simulating the module
5.Reviewing and Adjusting Logic
6.Finalizing the Design
```
**PROGRAM**
```
module EX5(din,a,b,c);
input[0:7]din;
output a;
output b;
output c;
assign a= din[4]|din[5]|din[6]|din[7];
assign b= din[2]|din[3]|din[6]|din[7];
assign c= din[2]|din[4]|din[6]|din[7]; 
endmodule
```

**RTL LOGIC FOR Encoder 8 To 3 in Dataflow Modelling**

![Screenshot 2025-05-08 083543](https://github.com/user-attachments/assets/29d56bb4-1146-47f1-abb1-0438c12a6b7a)

**TIMING DIGRAMS FOR Encoder 8 To 3 in Dataflow Modelling**

![Screenshot 2025-05-08 084819](https://github.com/user-attachments/assets/8607a68a-ed74-4068-a8f6-d5925117b045)

**RESULTS**

Therefore encoder 8 to 3 in dataflowing modeling using verilog and validating their functionality using their functional tables is verified.




