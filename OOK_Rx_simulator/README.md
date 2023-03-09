#### OOK_Rx_simulator
"OOK_Rx_simulator" shows how to demodulate on-off-keying (OOK) data by mixing the modulated signal with the carrier signal.  No external hardware needed.   

The baseband signal has 24-bits (0, 1, 0, 1, 0, 1, 0, 1, 1, 1, 0, 0, 0, 0, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0).  

![Signals](https://github.com/michaelalex94536/GRCProjects/blob/main/Images/OOK_Rx_Simulator_Signals.png)

From the constellation plot below, we see the 0's and 1's are distinguishable, even in the presence of moderate noise. 

![Signals](https://github.com/michaelalex94536/GRCProjects/blob/main/Images/OOK_Rx_Simulator_Constellation.png)

The GUI has a slider to change the Tx frequency and a slider to change the Rx frequency.  If you move the sliders around and then set them to the same frequency, you might see that the constellation points are no longer on the real (In-phase) axis.  This is because even though the Tx and Rx frequencies may be the same, the two sources are out of phase with respect to each other. 

To receive and demodulate an OOK signal (or virtually every other type of modulated signal) successfully in the real world, the receiver must lock-in to the correct modulation frequency AND phase.  More on this as we go along. 
