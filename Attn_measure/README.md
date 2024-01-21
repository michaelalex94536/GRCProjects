## Attn_measure

### Introduction
"Attn_measure" shows how to measure the attenuation of an in-line attenuator with the Pluto.  As seen in the photograph below, the attenuators used here (blue, barrel-shaped device in the upper-right portion of the figure) had SMA connectors that allowed them to be easily connected between the Tx and Rx SMA connectors of the Pluto using short SMA cables.  I used three attenuators made by a company called Mini-Circuits with attenuation values of 3dB, 8dB, and 10dB stamped on their bodies. Since the attenuators can be connected in series, I measured the Pluto Tx to Rx power loss for ideal attenuation values of 3dB, 8dB, 10dB, 11dB, 13dB, 18dB, and 21dB.  
&nbsp;  
![Signals](https://github.com/michaelalex94536/GRCProjects/blob/main/Images/Pluto_Attn.png)

Figure 1    Attenuator connected in-line between the Tx and Rx SMA connectors of the Pluto. This unit has been hacked to add additional Rx and Tx channels.  
<p>&nbsp;</p>

### Procedure
Using the GRC flowgraph associated with this project, the Tx and Rx SMA connectors of the Pluto were directly connected together with short cables. The Tx attenuation of the Pluto Sink and the Rx gain of the Pluto Source were adjusted so that the spectral peak of the 150kHz Signal Source was approximately -65dB. It is important the initial Rx gain and Tx attenuation are set such that the unattenuated 150kHz signal is not over-amplified and distorted (check the spectrum for harmonics!) but not too close to the noise floor either.  In my case, the Rx gain was set to 0dB and the Tx attenuation was set to 43dB.  In Figure 2 below, we see the 150kHz signal spectral peak and noise floor with no attenuators in use.  

![Signals](https://github.com/michaelalex94536/GRCProjects/blob/main/Images/PlutoAttenuator_spectrum.png)

Figure 2    Measured 150kHZ spectral peak with no attenuators in use. Here, the Pluto Tx attenuation and Rx gain were set to 43dB and 0 dB respectively.  
<p>&nbsp;</p>
