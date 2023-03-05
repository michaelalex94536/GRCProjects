
#### OOK_Tx_simulator
"OOK_Tx_simulator" shows how to modulate a carrier with digital data using on-off keying (OOK).  No external hardware needed.   

In OOK, the carrier signal is modulated by a baseband signal that is either a 0 or a 1, which turns the carrier on or off.  OOK is a form of ASK (amplitude-shift keying) in which there are only two amplitude levels, one of which is 0. 

https://en.wikipedia.org/wiki/On%E2%80%93off_keying



In this example, the baseband digital signal has 24-bits (0, 1, 0, 1, 0, 1, 0, 1, 1, 1, 0, 0, 0, 0, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0).  Here are 2 periods of the digital and transmitted data:

![Signals](https://github.com/michaelalex94536/GRCProjects/blob/main/Images/OOK_Tx_Simulator_Signals.png)

The constellation plot in the flowgraph clearly shows we only have 1' and 0's in the data pattern (not shown here).  T

