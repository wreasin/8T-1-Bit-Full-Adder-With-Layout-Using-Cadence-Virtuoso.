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

![Scametic_gif](https://github.com/wreasin/CMOS-XNOR-Gate-Design-using-Cadence-Virtuoso/blob/main/image/Scametic.gif?raw=true)
![Scametic](https://github.com/wreasin/CMOS-XNOR-Gate-Design-using-Cadence-Virtuoso/blob/main/image/Scametic.PNG?raw=true)
![Symbol](https://github.com/wreasin/CMOS-XNOR-Gate-Design-using-Cadence-Virtuoso/blob/main/image/Symbol.PNG?raw=true)
![Symbol_Scametic](https://github.com/wreasin/CMOS-XNOR-Gate-Design-using-Cadence-Virtuoso/blob/main/image/Symbol_Scametic.PNG?raw=true)

#### Transient, DC, AC & Noise Response :
_Here I am doing four types of Analysis - Transient, DC, AC & Noise_.  
In DC and Transient Analysis i have measured Va, Vb & Vout as Voltage, and Current (I) in VDD node. In AC Analysis i have measured Va, Vb & Vout as Voltage Frequency and Current (I) Frequency in VDD node. For DC and Transient Analysis the plots of _Va_ , _Vb_ and _Vout_ shows the _voltages_, on the otherhand _VDD(I4)_ shows the _current (I)_. For AC Analysis the plots of _Va_ , _Vb_ and _Vout_ shows the _voltage frequency_, on the otherhand _VDD(I4)_ shows the _current (I) frequency_. 
![output](https://github.com/wreasin/CMOS-XNOR-Gate-Design-using-Cadence-Virtuoso/blob/main/image/Output.PNG?raw=true)  
![output2](https://github.com/wreasin/CMOS-XNOR-Gate-Design-using-Cadence-Virtuoso/blob/main/image/Output_2.PNG?raw=true)

#### Calculating Power Consumption also Average Power of this circuit using Calculator. :  
For measuring of Noise Response, Noise Figure and Noise Factor i had to use PORTS instead of Vpulse. For Noise Analysis i have measured input, output & VN2 noise and also Noise Figure. In Noise Response the plots shows the input, output & VN2 noise and also Noise Figure.  
![noise_figure_scametic](https://github.com/wreasin/CMOS-XNOR-Gate-Design-using-Cadence-Virtuoso/blob/main/image/Noise%20Analysis_Scametic.PNG?raw=true)
![noise_output](https://github.com/wreasin/CMOS-XNOR-Gate-Design-using-Cadence-Virtuoso/blob/main/image/Noise_Output(IN.OUT,Noise%20Figure,Noise%20Factor).PNG?raw=true)
![noise_output_2](https://github.com/wreasin/CMOS-XNOR-Gate-Design-using-Cadence-Virtuoso/blob/main/image/Noise_Output(IN.OUT,Noise%20Figure,Noise%20Factor)_2.PNG?raw=true)

#### Layout :
In Layout i have use Metal1, Metal2 and Poly layer for gate. I have use here X & Y snap spacing is 0.005m and also the minimum width of metal utilized for routing is 0.12.  
![Layout_gif](https://github.com/wreasin/CMOS-XNOR-Gate-Design-using-Cadence-Virtuoso/blob/main/image/Layout.gif?raw=true)
![Layout](https://github.com/wreasin/CMOS-XNOR-Gate-Design-using-Cadence-Virtuoso/blob/main/image/Layout.PNG?raw=true)

#### Design Rule Check (DRC)  
DRC is clean. There are no error in DRC.
![DRC](https://github.com/wreasin/CMOS-XNOR-Gate-Design-using-Cadence-Virtuoso/blob/main/image/DRC%20Check.PNG?raw=true)  

#### Layout Versus Schematic (LVS)  
LVS is clean. There are no error in LVS.  
![LVS](https://github.com/wreasin/CMOS-XNOR-Gate-Design-using-Cadence-Virtuoso/blob/main/image/LVS%20Check.jpg?raw=true)
