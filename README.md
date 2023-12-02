# Experiment-08- Encoders-and-decoders 
### AIM: To implement 8 to 3 Encoder and  3to8 Decoder using verilog and validate its outputs
### Developed by:
J.Nandakesore

### Register Number:
23009689
### HARDWARE REQUIRED:  – PC, Cyclone II , USB flasher
### SOFTWARE REQUIRED:   Quartus prime
### THEORY 

## Encoders
Binary code of N digits can be used to store 2N distinct elements of coded information. This is what encoders and decoders are used for. Encoders convert 2N lines of input into a code of N bits and Decoders decode the N bits into 2N lines.

1. Encoders –
An encoder is a combinational circuit that converts binary information in the form of a 2N input lines into N output lines, which represent N bit code for the input. For simple encoders, it is assumed that only one input line is active at a time.

As an example, let’s consider Octal to Binary encoder. As shown in the following figure, an octal-to-binary encoder takes 8 input lines and generates 3 output lines.

![image](https://user-images.githubusercontent.com/36288975/171543588-bc0746df-a173-4b35-989e-5fb7d385fe8a.png)
## Figure -01 3 to 8 Encoder 


Implementation –

X = D4 + D5 + D6 + D7
Y = D2 +D3 + D6 + D7
Z = D1 + D3 + D5 + D7 
Hence, the encoder can be realised with OR gates as follows:


![image](https://user-images.githubusercontent.com/36288975/171543740-68403b82-aa93-4c98-9343-f32b14885a2e.png)
## Figure -02 3 to 8 Encoder implenentation 

 ### Decoders 
A decoder does the opposite job of an encoder. It is a combinational circuit that converts n lines of input into 2n lines of output.

Let’s take an example of 3-to-8 line decoder.
Implementation –
D0 is high when X = 0, Y = 0 and Z = 0. Hence,

D0 = X’ Y’ Z’ 
Similarly,

D1 = X’ Y’ Z
D2 = X’ Y Z’
D3 = X’ Y Z
D4 = X Y’ Z’
D5 = X Y’ Z
D6 = X Y Z’
D7 = X Y Z 


![image](https://user-images.githubusercontent.com/36288975/171543978-ee2d0671-2846-40a1-8705-507fd6287a49.png)
## Figure -03 8 to 3 Decoder 



![image](https://user-images.githubusercontent.com/36288975/171543866-5a6eace6-8683-49d7-9c4f-a7cb30ec3035.png)
## Figure -04 8 to 3 Decoder implementation 

### Procedure
1.create module encoder and decoder.

2.Get inputs and outputs for encoders and decoders.

3.perform or operation for encoder and and logic for decoders.

4.perform RTL LOGIC and get waveform.

### PROGRAM 

## Encoder:

![image](https://github.com/Nandakesore0210/Experiment-08-Encoders-and-decoders-/assets/149365088/eff98ebf-7091-4ab7-9f3a-698ad75837dd)

## Decoder:

![image](https://github.com/Nandakesore0210/Experiment-08-Encoders-and-decoders-/assets/149365088/9c45b126-ecfe-4166-9b30-f676866b06ad)

### RTL LOGIC  

## Encoder:

![image](https://github.com/Nandakesore0210/Experiment-08-Encoders-and-decoders-/assets/149365088/44c9a167-8f5c-482c-8dfc-4ae8b462a5b4)

## Decoder:

![image](https://github.com/Nandakesore0210/Experiment-08-Encoders-and-decoders-/assets/149365088/3849e5b6-7600-4042-b18e-ba8460703931)

### TIMING DIGRAMS  

## Encoder:

![image](https://github.com/Nandakesore0210/Experiment-08-Encoders-and-decoders-/assets/149365088/fe508823-0032-47a7-a99a-58dedc196d48)

## Decoder:

![image](https://github.com/Nandakesore0210/Experiment-08-Encoders-and-decoders-/assets/149365088/80294900-2a83-478e-86ba-6f8c99d79a46)

### TRUTH TABLE 

## Encoder:

![image](https://github.com/Nandakesore0210/Experiment-08-Encoders-and-decoders-/assets/149365088/22392403-e336-453c-8f6c-f2cde3b889f6)

## Decoder:

![image](https://github.com/Nandakesore0210/Experiment-08-Encoders-and-decoders-/assets/149365088/055145b0-8220-45fd-8ef5-1b9fe224a1a3)

### RESULTS:

Thus the program to desing encoder and decoder is done.
