
#### OOK_decoder
"OOK_decoder" takes an IQ data file captured in the "OOK_capture" project and shows the signals in both time- and frequency domians, in addition to the baseband signal constellation.  In this project we attempt to decode the baseband garage door opener signals.  As the IQ data is provided in a zip file, no external hardware is required.  

Figure 1 below shows a zoom of the time domain IQ data that was captured in the "OOK_capture" project.  Holy smokes - the data is not simply OOK - it appears to be Binary FSK modulated (BFSK).  I haven't been able to find any information on this type of decoding for such old garage door openers.  In retrospect, the spectrum seemed to have more than one peak, so I'm not surprised.  I'm still trying to figure the modulation out and will update this project when I do. 

#### Figure 1     Complex signal from garage door opener captured using RTL-SDR dongle.  It does not appear to be simple OOK.
![Model](https://github.com/michaelalex94536/GRCProjects/blob/main/Images/decoded_image.png)

