#### Real_vs_complex_signals

In this project, we show the frequency spectra of the product of real and complex signals.  The results may be a bit surprising.  

Since we are just looking at signals such as sines and cosines at fixed frequencies, we expect the spectra of such signals to exhibit "spikes" or delta functions at those frequencies.  

Now, a real signal has both negative and positive frequencies.  When two real signals are multiplied, the products are located at both the sum and difference frequencies of the two signals, and these sum and difference frequencies are seen at both positive and negative frequencies - which means there are four peaks in the product spectrum, as seen in the figure below,  where we show the product spectrum of two sinusoidal signals having frequencies of 100kHz and 200kHz, respectively.  The difference frequencies +/-100kHz and +/-300kHz are clearly seen.  If we change the sign of the signals, the spectral peaks remain at their original positions.  In other words, we can't tell whether the original real time-domain signals A and B had positive or negative frequencies.  
![image](https://github.com/michaelalex94536/GRCProjects/blob/main/Images/real_signal_product_spectrum.png)

On the other hand, a complex sinusoidal signal has only one peak in its spectrum.  Yes, hard to believe, but it is true.  Furthermore, the product of two complex sinusoids having different frequencies has a spectrum exhibiting one peak at a frequency which is the sum of the two frequencies.  Here is the spectrum of the product of two complex signals having the same frequencies as in the figure above: 
![image](https://github.com/michaelalex94536/GRCProjects/blob/main/Images/complex_signal_product_spectrum.png)

Finally, we see that when we change the sign(s) of the frequencies of the original complex time-domain signals A or B, the sign of the frequency on the spectral axis changes sign as well.  

From "Signal_Generator" project README.md:

From Euler's formula, a real signal described by a cosine of a given frequency can be written as a pair of phasors whose frequencies have opposite sign, giving rise to the two peaks at positive and negative frequencies seen in the figure above:

![image](https://github.com/michaelalex94536/GRCProjects/blob/main/Images/real_signal_eqn.png)

For the complex signal, it is easy to show the negative frequency terms cancel, leading to a single peak at a positive frequency: 

![image](https://github.com/michaelalex94536/GRCProjects/blob/main/Images/complex_signal_eqn.png)  

