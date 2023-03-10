
#### ASK_Rx_simulator
"ASK_Rx_simulator" shows how to demodulate amplitude-shift keying (ASK) data by mixing the modulated signal with the carrier signal.  No external hardware needed.  The constellation plot shows we have 4 clusters of signals - the 4 diffferent amplitudes of the baseband ASK data with additive noise.  

Note that if you change the frequency in this project, the constellation will probably rotate.  This is because even though the Tx frequency and the Rx (demodulation) frequencies are the same, the sampling phase has changed.  

![Signals](https://github.com/michaelalex94536/GRCProjects/blob/main/Images/ASK_Rx_Simulator_Constellation.png)


