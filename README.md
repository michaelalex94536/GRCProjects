# GRCProjects

## GRC projects I've put together

#### Developed and tested using GNU Radio Companion 3.10.1.1 on a Linux system using Ubuntu 22.04.2 LTS.  Many of the projects require the use of an RTL-SDR dongle (or equivalent) for capturing signals from the air.  Each project folder contains a *.grc file, a corresponding *.py file, a *.pdf file that shows the project flowgraph and a README.md file.  Some folders might contain several related projects.  

#### For projects that require signal transmission, we will use a HackRF or an ADALM-Pluto. Each project description below gives more details about what the project requires, as well as a brief explanation of what's going on.  Projects are listed in no special order, but I've tried to keep the ones that don't require external hardware near the top. 

### Project descriptions 

#### Signal_generator
Real and complex signals are generated and displayed in the time- and frequency domains.  No external hardware is required for this project. 

#### DTMF_generator
The "DTMF_generator" project generates DTMF (Touch-Tone) signals, displays them in the time and frequency domains, and plays the Touch-Tones using the PC speaker. No external hardware is required for this project. 

#### OOK_Tx_simulator
"OOK_Tx_simulator" shows how to modulate a carrier with digital data using on-off-keying.  No external hardware needed.   

#### OOK_Rx_simulator
"OOK_Rx_simulator" shows how to very naively demodulate a carrier with digital data using on-off-keying.  No external hardware needed.  



#### OOK_capture
"OOK_capture" shows how to use an RTL-SDR dongle to display and capture OOK signals from a very old garage door opener. 

#### OOK_decoder
"OOK_decoder" takes an IQ data file captured in the "OOK_capture" project and shows the signals in both time- and frequency domains.  No hardware needed as we use IQ data previously captured and stored in a file.  

#### FM_receiver_basic
"FM_receiver_basic" shows how to use an RTL-SDR dongle to demodulate and listen to a single, user-selected FM radio station using the PC speaker.
