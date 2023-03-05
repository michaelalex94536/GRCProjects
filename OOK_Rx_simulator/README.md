#### OOK_Rx_simulator
"OOK_Rx_simulator" shows how to naively demodulate an on-off-keying (OOK).  No external hardware needed.   

The baseband signal has 24-bits (0, 1, 0, 1, 0, 1, 0, 1, 1, 1, 0, 0, 0, 0, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0).  If you freeze the stem plot of the flowgraph (triggering is tricky) you can confirm the digital pattern. 

![Signals](https://github.com/michaelalex94536/GRCProjects/blob/main/Images/OOK_Rx_Simulator_Signals.png)


Note that in order to recover the bits, we downsample the demodulated signal (using the GRC "Keep 1 in N" block) with the same rate at which we upsampled the data when it was "transmitted" (using the "samps_pre_sym" value in the GRC "Repeat" block). 
