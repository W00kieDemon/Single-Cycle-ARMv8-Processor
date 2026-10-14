# D Latch Overview
The purpose of the SR Latch is to introduce the most basic form of computer memory so that we can manipulate data. The D-latch itself is a form of 1-bit memory, meaning it maintains the state of a single bit; that state being on or off. By definition, this circuit must be sequential in nature because he relies on it's previous state to determine it's current state. 
## Circuit Design
Let me begin by stating this circuit has been designed previously, however this document is attempting to walk through some of the logic you'd consider if you were designing this circuit from scratch. We can start by clearly laying out exactly what we want the circuit to do, then design the circuit accordingly. We can imagine a black box circuit right now, one that outputs a single bit of data based on it's previous state. We'll need at one input to set the data, and one input to tell the circuit when it should remember and when it should set. We call this latching, hence the name "D-Latch". We'll all the input bit telling the circuit what state to latch data, or D for short, and we'll call the input telling the circuit when to remember enable because it's enabling the latch, or En for short. We can pick an arbitrary value to tell the latch when to remember, but because intuitively we consider 1 to be True or Yes and 0 to be False or No, we will determine the circuit should latch on a high enable. This is a lot of information, so for simplicity, here is a truth table for the overall circuit we'd like to design:
|En|D|Out|
|0|0|Prev|
|0|1|Prev|
|1|0|0|
|1|1|1|
