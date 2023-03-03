# GRCProjects

## GRC projects I've put together

#### Developed and tested using GNU Radio Companion 3.10.1.1 on a Linux system using Ubuntu 22.04.2 LTS.  Many of the projects require the use of an RTL-SDR dongle (or equivalent) for capturing signals from the air.  Each folder contains a project with a *.grc file, a corresponding *.py file, and a *.pdf file that shows the project blocks layout; some folders may also have image files. The only file one really needs is the *.grc file. Some folders might contain multiple, related projects.  

#### For projects that require signal transmission, we will use a HackRF or an ADALM-Pluto. Each project description below gives more details about what the project requires, as well as a brief explanation of what's going on.  Projects are listed in no special order, but I've tried to keep the ones that don't require external hardware near the top. 

### Project descriptions 
#### DTMF_generator
The "DTMF_generator" project generates DTMF (Touch-Tone) signals, displays them in the time and frequency domains, and plays the Touch-Tones using the PC speaker. No external hardware required. This flowgraph is just a gentle introduction to GNU Radio Companion basics.

#### OOK_capture
"OOK_capture" shows how to use an RTL-SDR dongle to display OOK signals from a very old garage door opener, in this case one having a carrier frequency of approximately 390 MHz. The user should set the appropriate frequency for their device (it's usually written on the device somewhere), and don't forget to use an antenna with the SDR dongle. The time and frequency domain OOK signals are shown, along with the constellation plot, which is pretty simple in this case. We also compute the magnitude of the complex time domain signal, decimate it, and show it in the time domain - allowing us to clearly see the 0's and 1's that were transmitted. The decimated signal is also sent to an audio sink - the PC speaker - so we can hear the bursts generated when the garage door opener button is pushed.  Finally, there is a file sink block in case the user wants to save the captured IQ data. In addition to an RTL-SDR dongle (or other hardware) for signal capture, the user will need a garage door opener or key fob to generate the OOK signals. Note: depending on receiver gain settings and distance from the key fob to the receiver, the received signal may saturate or clip. The folder also includes IQ data from my garage door opener in a zip file.  

#### OOK_decoder
"OOK_decoder" takes an IQ data file captured in the "OOK_capture" project and shows the signals in both time- and frequency domians, in addition to the baseband signal constellation.  In this project we attempt to decode the baseband garage door opener signals.  As the IQ data is provided in a zip file, no external hardware is required.  

The image below shows a zoom of the time domain IQ data that was captured in the "OOK_capture" project.  Holy smokes - the data is not simply OOK - it appears to be Binary FSK modulated (BFSK).  I haven't been able to find any information on this type of decoding for such old garage door openers.  In retrospect, the spectrum seemed to have more than one peak, so I'm not surprised.  

![Model](https://github.com/michaelalex94536/GRCProjects/blob/main/OOK_decoder/ksnip_20230302-182412.png)

#### FM_receiver_basic
"FM_receiver_basic" shows how to use an RTL-SDR dongle to demodulate and listen to a single, user-selected FM radio station.  This project uses the GRC wide band FM demodulator (WBFM Receive) block.  The user selects the FM station frequency using a slider.  Various time- and frequency-domain signals are displayed. 
