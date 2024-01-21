## Attn_measure

### Introduction
"Attn_measure" shows how to measure the attenuation of an in-line attenuator with the Pluto.  As seen in the photograph below, the attenuators used here (blue, barrel-shaped device in the upper-right portion of the figure) had SMA connectors that allowed them to be easily connected between the Tx and Rx SMA connectors of the Pluto using short SMA cables.  I used three attenuators made by a company called Mini-Circuits with attenuation values of 3dB, 8dB, and 10dB stamped on their bodies. Since the attenuators can be connected in series, I measured the Pluto Tx to Rx power loss for ideal attenuation values of 3dB, 8dB, 10dB, 11dB, 13dB, 18dB, and 21dB.  
&nbsp;  
![Signals](https://github.com/michaelalex94536/GRCProjects/blob/main/Images/Pluto_Attn.png)

Figure 1    Attenuator connected in-line between the Tx and Rx SMA connectors of the Pluto. This unit has been hacked to add additional Rx and Tx channels.  
<p>&nbsp;</p>

### Procedure
Using the GRC flowgraph associated with this project (PlutoFilterTester.grc), the Tx and Rx SMA connectors of the Pluto were directly connected together with short cables. The Tx attenuation of the Pluto Sink and the Rx gain of the Pluto Source were adjusted so that the spectral peak of the 150kHz Signal Source was approximately -39dB. It is important the initial Rx gain and Tx attenuation are set such that the unattenuated 150kHz signal is not over-amplified and distorted (check the spectrum for harmonics!) but not too close to the noise floor either.  In my case, the Rx gain was set to 0dB and the Tx attenuation was set to 43dB.  In Figure 2 below, we see the 150kHz signal spectral peak and noise floor with high attenuation; since we started at -39dB, the attenuated signal is still well-above the noise floor.  The Rx gain and Tx attenuation settings in the flowgraph must be held fixed for all subsequent measurements, of course.   

![Signals](https://github.com/michaelalex94536/GRCProjects/blob/main/Images/PlutoAttenuator_spectrum.png)

Figure 2    Measured 150kHZ spectral peak with high attenuation in use. Here, the Pluto Tx attenuation and Rx gain were set to 43dB and 0 dB respectively.  
<p>&nbsp;</p>

Once appropriate Rx gain and Tx attenuation settings for the flowgraph are found, the magnitude of the 150kHz spectral peak is recorded without any attenuation, and then the attenuators are connected between the Pluto Tx and Rx connectors and the spectral peak magnitude is recorded.  I swapped out the attenuators with the flowgraph turned off for safety, started the flowgraph, and then put the mouse cursor on the 150kHz peak to estimate the power in the signal; I'm sure there is a much smarter way to do this in the flowgraph.  One can then make a table of the measured power versus the attenuation value and subtract the 0dB attenuation spectral peak value from all measurements in order to plot the measured versus the ideal attenuation as seen in Figure 3 below. 

![Signals](https://github.com/michaelalex94536/GRCProjects/blob/main/Images/PlutoAttenuator_plot.png)
