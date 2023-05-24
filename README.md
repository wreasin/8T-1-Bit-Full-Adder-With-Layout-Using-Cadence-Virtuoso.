# 8T 1-Bit Full Adder Design Using Cadence Virtuoso
### 8T 1-Bit Full Adder Design and Analysis With Layout Using Cadence Virtuoso

---
<!-- Cadence Project (Transient, DC, AC, Noise Response, Power Consumption (Average Power) With Layout) -->

I’m really glad to share that, this is my seventh project on __Cadence Virtuoso__. I am designing here a 8T 1-Bit Full Adder Design and Analysis With Layout Using Cadence Virtuoso.

___Before I start explaining my project in details, you should know a few things !___     

### What is 8T 1-Bit Full Adder?  
An 8T 1-bit full adder is a digital circuit that is used to perform binary addition of two 1-bit numbers along with an input carry bit, resulting in a 1-bit sum and a carry output. The 8T in the name refers to the eight transistors that are used in the circuit implementation.

The 8T 1-bit full adder circuit is designed using a combination of PMOS and NMOS transistors. The circuit uses four PMOS transistors and four NMOS transistors, with each transistor having specific dimensions (width and length) based on the technology node of the fabrication process being used.

The 8T 1-bit full adder circuit can be represented by the following Boolean expression:

Sum (S) = A ⊕ B ⊕ Cin

Carry (Cout) = (A AND B) OR (Cin AND (A ⊕ B))

Where A, B, and Cin are the binary input bits representing the two numbers to be added and the carry-in bit, respectively, and S and Cout are the binary output bits representing the sum and carry-out bit, respectively.

The 8T 1-bit full adder circuit consists of three stages: a first stage, a second stage, and a third stage. The first stage of the circuit is a XOR gate, which is used to perform the addition of the two input bits (A and B). The second stage of the circuit is a second XOR gate, which is used to add the carry bit (Cin) to the sum produced by the first stage. The third stage of the circuit is an OR gate, which combines the outputs of the first and second stages to produce the final sum and carry outputs.
In the 8T 1-bit full adder circuit, each transistor is designed to operate in either the cut-off or saturation region, depending on the input signals. The circuit is designed to operate with a single supply voltage, which is typically in the range of 1-1.2V.

### The Project details of mine :

I'm using 45nm GPDK :-

1 ) Four pMOS1v & Four nMOS1v.  
2 ) Here i am doing four types of Analysis :  
    i ) Transient Response  
ii ) DC Response  
iii ) AC Response  
iv ) Noise Response  
3 ) I'm Calculated the Power Consumption (Average Power) of this circuit using Calculator.  
4 ) In Layout - Metals Used ( Metal1, Metal2 & Poly for gate )  
5 ) DRC and LVS clean (there are no error)

So I designed a Schematic of the 8T 1-Bit Full Adder, where the whole thing is based on gpdk45nm. I have use 4 PMOS1v & 4 NMOS1v. I also designed a symbol of it, so that i can utilise that for further schematic creation.  

The below figure shows a 8T 1-Bit Full Adder Circuit.  

![Scametic](https://github.com/wreasin/8T-1-Bit-Full-Adder-With-Layout-Using-Cadence-Virtuoso./blob/main/Image/Scametic.PNG)
![Symbol](https://github.com/wreasin/8T-1-Bit-Full-Adder-With-Layout-Using-Cadence-Virtuoso./blob/main/Image/Symbol.PNG)

#### Transient, DC, AC & Noise Response :
_Here I am doing four types of Analysis - Transient, DC, AC & Noise_.  
In DC and Transient Analysis i have measured Va, Vb & Vout as Voltage, and Current (I) in VDD node. In AC Analysis i have measured Va, Vb & Vout as Voltage Frequency and Current (I) Frequency in VDD node. For DC and Transient Analysis the plots of _Va_ , _Vb_ and _Vout_ shows the _voltages_, on the otherhand _VDD(I4)_ shows the _current (I)_. For AC Analysis the plots of _Va_ , _Vb_ and _Vout_ shows the _voltage frequency_, on the otherhand _VDD(I4)_ shows the _current (I) frequency_. 
![Symbol_Scametic](https://github.com/wreasin/8T-1-Bit-Full-Adder-With-Layout-Using-Cadence-Virtuoso./blob/main/Image/Symbol_Scametic.PNG)
![output](https://github.com/wreasin/8T-1-Bit-Full-Adder-With-Layout-Using-Cadence-Virtuoso./blob/main/Image/Transient_AC_DC_Noise%20Analysis.PNG) 

#### Calculating Power Consumption also Average Power of this circuit using Calculator. :  
Calculating Power Consumption Calculator for an 8T 1-bit Full Adder. The calculator allows you to calculate both the total power consumption and the average power of the circuit. By inputting relevant parameters, you can quickly determine the power requirements of the circuit, aiding in design and optimization processes.  
![All Power Consumption](https://github.com/wreasin/8T-1-Bit-Full-Adder-With-Layout-Using-Cadence-Virtuoso./blob/main/Image/All%20Power%20Consumption.PNG)
![Sum Carry_Aver_Power Consumption](https://github.com/wreasin/8T-1-Bit-Full-Adder-With-Layout-Using-Cadence-Virtuoso./blob/main/Image/Sum_Carry_Aver_Power%20Consumption.PNG)
![Sum Power Consumption](https://github.com/wreasin/8T-1-Bit-Full-Adder-With-Layout-Using-Cadence-Virtuoso./blob/main/Image/Sum%20Power%20Consumption.PNG) 
![Carry Power Consumption](https://github.com/wreasin/8T-1-Bit-Full-Adder-With-Layout-Using-Cadence-Virtuoso./blob/main/Image/Carry%20Power%20Consumption.PNG)

#### Layout :
In Layout i have use Metal1, Metal2 and Poly layer for gate. I have use here X & Y snap spacing is 0.005m and also the minimum width of metal utilized for routing is 0.12.  
![Layout](https://github.com/wreasin/8T-1-Bit-Full-Adder-With-Layout-Using-Cadence-Virtuoso./blob/main/Image/Layout.PNG)

#### Design Rule Check (DRC)  
DRC is clean. There are no error in DRC.  
![DRC](https://github.com/wreasin/8T-1-Bit-Full-Adder-With-Layout-Using-Cadence-Virtuoso./blob/main/Image/DRC%20Cheack.PNG)

#### Layout Versus Schematic (LVS)  
LVS is clean. There are no error in LVS.  
![LVS](https://github.com/wreasin/8T-1-Bit-Full-Adder-With-Layout-Using-Cadence-Virtuoso./blob/main/Image/LVS%20Cheack.PNG)
