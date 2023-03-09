#### OOK_Rx_simulator
"OOK_Rx_simulator" shows how to demodulate on-off-keying (OOK) data by mixing the modulated signal with the carrier signal.  No external hardware needed.   

The baseband signal has 24-bits (0, 1, 0, 1, 0, 1, 0, 1, 1, 1, 0, 0, 0, 0, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0).  

![Signals](https://github.com/michaelalex94536/GRCProjects/blob/main/Images/OOK_Rx_Simulator_Signals.png)

From the constellation plot below, we see the 0's and 1's are distinguishable, even in the presence of moderate noise. 

![Signals](https://github.com/michaelalex94536/GRCProjects/blob/main/Images/OOK_Rx_Simulator_Constellation.png)

The GUI has a slider to change the Tx frequency and a slider to change the Rx frequency.  If you move the sliders and set them to different frequencies relative to each other, you will see the sample points for the digit "1" spin around the unit circle at a frequency which is equal to the difference in frequency of the two sliders.   

If you move both the sliders and set them to the same frequency, you might see that the constellation points are no longer on the real (In-phase) axis.  This is because even though the Tx and Rx frequencies may be the same - and the sample constellations are no longer rotating - the receiver phase has shifted relative to the transmitted signal phase. 

To receive and demodulate an OOK signal (or virtually every other type of modulated signal) successfully in the real world, the receiver must lock-in to the correct modulation frequency AND phase.  More on this as we go along. 
