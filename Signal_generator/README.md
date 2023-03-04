
#### Signal_generator

No external hardware needed.

In this flowgraph, we use the GRC Signal Source block to create a complex signal with a frequency of the user's choosing, and display it in the time- and frequency-domains.  We also take the conjugate of the complex signal and add it to itself, eliminating the complex portion of the signal, leaving only a real signal.  We also display the real signal in the time- and frequency domains.  

Here is what we see for 5kHz signals, where the complex signal plots are on the left hand side of the figure, and the real signal results are on the right hand side. 

![Model](https://github.com/michaelalex94536/GRCProjects/blob/main/Images/Complex_Real_plots.png)

We note the real signal has two peaks in its frequency spectrum, one at a positive frequency and one at a negative frequency, while the complex signal has only one peak at the positive frequency.  This may come across as confusing to some people, so an explanation is in order. 

From Euler's formula, a real signal described by a cosine of a given frequency can be written as a pair of phasors whose frequencies have opposite sign, giving rise to the two peaks at positive and negative frequencies seen in the figure above:

![image](https://github.com/michaelalex94536/GRCProjects/blob/main/Images/real_signal_eqn.png)

For the complex signal, it is easy to show the negative frequency terms cancel, leading to a single peak at a positive frequency: 

![image](https://github.com/michaelalex94536/GRCProjects/blob/main/Images/complex_signal_eqn.png)  

