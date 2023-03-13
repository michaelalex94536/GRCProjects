#### Real_vs_complex_signals

In this project, we show the frequency spectra of the product of real and complex signals.  The results may be a bit surprising.  

Since we are just looking at signals such as sines and cosines at fixed frequencies, we expect the spectra of such signals to exhibit "spikes" or delta functions at those frequencies.  

A real signal has both negative and positive frequencies.  When two real signals are multiplied, the products are located at both the sum and difference frequencies of the two signals, and these sum and difference frequencies are seen at both positive and negative frequencies - which means there are four peaks in the product spectrum, as seen in the figure below,  where we show the product spectrum of two sinusoidal signals having frequencies of 100kHz and 200kHz, respectively.  The difference frequencies +/-100kHz and +/-300kHz are clearly seen.  
![image](https://github.com/michaelalex94536/GRCProjects/blob/main/Images/real_signal_product_spectrum.png)

Now, a complex sinusoidal signal has only one peak in its spectrum.  Yes, hard to believe, but it is true.  Furthermore, the product of two complex sinusoids having different frequencies has a spectrum exhibiting one peak at a frequency which is the sum of the two frequencies.  Here is the spectrum of the product of two complex signals having the same frequencies as in the figure above: 
![image](https://github.com/michaelalex94536/GRCProjects/blob/main/Images/complex_signal_product_spectrum.png)
