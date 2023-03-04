
#### Signal_generator
In this flowgraph, we use the GRC Signal Source block to create a complex signal with a frequency of the user's choosing, and display it in the time- and frequency-domains.  We also take the conjugate of the complex signal and add it to itself, eliminating the complex portion of the signal, leaving only a real signal.  We also display the real signal in the time- and frequency domains.  Here are typical results: 

![Model](https://github.com/michaelalex94536/GRCProjects/blob/main/Images/Complex_Real_plots.png)

We note the real signal has two peaks in its frequency spectrum, one at a positive frequency and one at a negative frequency, while the complex signal has only one peak at the positive frequency.  This may come across as confusing to some people, so an explanation is in order.  
![image](https://user-images.githubusercontent.com/26451874/222878726-ae09c08f-b8d7-4c65-9c42-96c51ff09063.png)

{func cos %phi} = { 1 } over {2} {[{func e}^{i %phi} + {func e}^{-i %phi}]}

