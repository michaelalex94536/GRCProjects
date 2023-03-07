#### OOK_Rx_simulator
"OOK_Rx_simulator" shows how to naively demodulate on-off-keying (OOK) data.  No external hardware needed.   

The baseband signal has 24-bits (0, 1, 0, 1, 0, 1, 0, 1, 1, 1, 0, 0, 0, 0, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0).  If you freeze the stem plot of the flowgraph (triggering is tricky) you can confirm the digital pattern. 

![Signals](https://github.com/michaelalex94536/GRCProjects/blob/main/Images/OOK_Rx_Simulator_Signals.png)


To receive and demodulate an OOK signal successfully in the real world, we need to determine the symbol time - the duration of a 1 or a 0.  
