NAME: RAMYA R

REG NO: 23000505

# Exp-6-Synchornous-counters - up counter and down counter 
### AIM: To implement 4 bit up and down counters and validate  functionality.
### HARDWARE REQUIRED:  – PC, Cyclone II , USB flasher
### SOFTWARE REQUIRED:   Quartus prime
### THEORY 

## UP COUNTER 
The counter is a digital sequential circuit and here it is a 4 bit counter, which simply means it can count from 0 to 15 and vice versa based upon the direction of counting (up/down). 

The counter (“count“) value will be evaluated at every positive (rising) edge of the clock (“clk“) cycle.
The Counter will be set to Zero when “reset” input is at logic high.
The counter will be loaded with “data” input when the “load” signal is at logic high. Otherwise, it will count up or down.
The counter will count up when the “up_down” signal is logic high, otherwise count down

Since we know that binary count sequences follow a pattern of octave (factor of 2) frequency division, and that J-K flip-flop multivibrators set up for the “toggle” mode are capable of performing this type of frequency division, we can envision a circuit made up of several J-K flip-flops, cascaded to produce four bits of output.
The main problem facing us is to determine how to connect these flip-flops together so that they toggle at the right times to produce the proper binary sequence.
Examine the following binary count sequence, paying attention to patterns preceding the “toggling” of a bit between 0 and 1:
Binary count sequence, paying attention to patterns preceding the “toggling” of a bit between 0 and 1.

Note that each bit in this four-bit sequence toggles when the bit before it (the bit having a lesser significance, or place-weight), toggles in a particular direction: from 1 to 0.



 
 

Starting with four J-K flip-flops connected in such a way to always be in the “toggle” mode, we need to determine how to connect the clock inputs in such a way so that each succeeding bit toggles when the bit before it transitions from 1 to 0.

The Q outputs of each flip-flop will serve as the respective binary bits of the final, four-bit count:

 
 

Four-bit “Up” Counter
![image](https://user-images.githubusercontent.com/36288975/169644758-b2f4339d-9532-40c5-af40-8f4f8c942e2c.png)



## DOWN COUNTER 

As well as counting “up” from zero and increasing or incrementing to some preset value, it is sometimes necessary to count “down” from a predetermined value to zero allowing us to produce an output that activates when the zero count or some other pre-set value is reached.

This type of counter is normally referred to as a Down Counter, (CTD). In a binary or BCD down counter, the count decreases by one for each external clock pulse from some preset value. Special dual purpose IC’s such as the TTL 74LS193 or CMOS CD4510 are 4-bit binary Up or Down counters which have an additional input pin to select either the up or down count mode.
![image](https://user-images.githubusercontent.com/36288975/169644844-1a14e123-7228-4ed8-81a9-eb937dff4ac8.png)


4-bit Count Down Counter
### Procedure
/* write all the steps invloved */



### PROGRAM 
/*
Program for flipflops  and verify its truth table in quartus using Verilog programming.

Developed by: Ramya R

RegisterNumber: 23000505

UP COUNTER

![Screenshot 2023-12-02 162518](https://github.com/ramya23000505/Exp-7-Synchornous-counters-/assets/149370791/b843ec17-d8ef-47c6-86ff-93dbbd26ed2d)

DOWN COUNTER

![Screenshot 2023-12-02 162534](https://github.com/ramya23000505/Exp-7-Synchornous-counters-/assets/149370791/17eb9627-a482-427f-8d89-dd98ff1d556d)

*/

### RTL LOGIC UP COUNTER AND DOWN COUNTER  

RLT FOR UP COUNTER

![Screenshot 2023-12-02 162548](https://github.com/ramya23000505/Exp-7-Synchornous-counters-/assets/149370791/60209423-d85b-4092-b78f-6a8ed29f5cbe)

RLT FOR DOWN COUNTER

![Screenshot 2023-12-02 162613](https://github.com/ramya23000505/Exp-7-Synchornous-counters-/assets/149370791/e6561dde-e46b-48f5-a0a0-aa545befdb4a)

### TRUTH TABLE 

TRUTH TABLE FOR UP COUNTER

![Screenshot 2023-12-02 162751](https://github.com/ramya23000505/Exp-7-Synchornous-counters-/assets/149370791/f00141fe-c5e1-4ed8-a070-15fcd9c485e8)

TRUTH TABLE FOR DOWN COUNTER

![Screenshot 2023-12-02 162829](https://github.com/ramya23000505/Exp-7-Synchornous-counters-/assets/149370791/86b1a271-ca49-41fc-89ea-6117439a4cf7)

### TIMING DIGRAMS FOR COUNTER  

TIMING DIGRAM FOR UP COUNTER 

![Screenshot 2023-12-02 162633](https://github.com/ramya23000505/Exp-7-Synchornous-counters-/assets/149370791/e3e6f449-3094-478b-a26d-f47141626464)

TIMING DIGRAM FOR DOWN COUNTER 

![Screenshot 2023-12-02 162644](https://github.com/ramya23000505/Exp-7-Synchornous-counters-/assets/149370791/fd7c630b-01bf-481d-9963-23c1bb578801)


### RESULTS 
