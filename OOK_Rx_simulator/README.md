#### OOK_Rx_simulator
"OOK_Rx_simulator" shows how to demodulate on-off-keying (OOK) data by mixing the modulated signal with the carrier signal.  No external hardware needed.   

The baseband signal has 24-bits (0, 1, 0, 1, 0, 1, 0, 1, 1, 1, 0, 0, 0, 0, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0).  

![Signals](https://github.com/michaelalex94536/GRCProjects/blob/main/Images/OOK_Rx_Simulator_Signals.png)

From the constellation plot below, we see the 0's and 1's are distinguishable, even in the presence of moderate noise. 

![Signals](https://github.com/michaelalex94536/GRCProjects/blob/main/Images/OOK_Rx_Simulator_Constellation.png)

To receive and demodulate an OOK signal successfully in the real world, we need to determine the symbol time - the duration of a 1 or a 0, as well as lock-in to the correct modulation frequency AND phase.  
