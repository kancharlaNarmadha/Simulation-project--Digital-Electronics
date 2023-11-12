# TITTLE
8 BIT PARITY GENERATOR USING VERILOG


# AIM:

Design and generate 8 bit parity generator using Verilog.

# EQUIPMENTS REQUIRED

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

# THEORY

Parity Generator
An 8-bit parity generator is a digital circuit that generates a parity bit based on a set of 8 input data bits. The purpose of the parity bit is to provide error detection in data transmission or storage systems.The parity bit is calculated based on the number of 1s in the input data bits. There are two types of parity: even parity and odd parity.In even parity, the parity bit is set to 1 if the number of 1s in the input data is odd. This ensures that the total number of 1s, including the parity bit, is always even.In odd parity, the parity bit is set to 1 if the number of 1s in the input data is even. This ensures that the total number of 1s, including the parity bit, is always odd.


# TRUTH TABLE

![Screenshot (321)](https://github.com/Anusharonselva/Simulation-project--Digital-Electronics/assets/119405600/5a870740-2dbc-48fb-862b-b2c3e5542c7d)


# LOGIC DIAGRAM

![Screenshot (322)](https://github.com/Anusharonselva/Simulation-project--Digital-Electronics/assets/119405600/d414289b-cd58-4e35-8e39-6af42ddcf55a)


# NETLIST DIAGRAM

![Screenshot (323)](https://github.com/Anusharonselva/Simulation-project--Digital-Electronics/assets/119405600/3ef73b2c-b07f-4508-934a-f05964294706)

# TIMING DIAGRAM

![Screenshot (324)](https://github.com/Anusharonselva/Simulation-project--Digital-Electronics/assets/119405600/58fb7048-00e6-4f2e-8c03-33210b1a8b8a)

# PROGRAM
 Program to simulate 8 bit parity generator using Verilog.
 NAME : S.ANUSHARON
 REG.NO : 212222240010


 module parity_generator (
       input [7:0] data_in,
       output reg parity_out
   );



   always @(*) 
        begin
           reg [7:0] xor_result;
  
          xor_result = data_in[0] ^ data_in[1] ^ data_in[2] ^ data_in[3] ^ data_in[4] ^ data_in[5] ^ data_in[6] ^ data_in[7];
           parity_out= ~xor_result;
             end

    endmodule

# RESULT
Thus the synchronous 8 bit parity generator has been implemented in Quartus Prime and output is verified by using Verilog programming through its truth table
