# GRCProjects

## GNU Radio Companion (GRC) projects

#### All projects listed here were developed and tested using GNU Radio Companion 3.10.1.1 on a Linux system using Ubuntu 22.04.2 LTS.  Some of the projects require the use of an RTL-SDR dongle (or equivalent) for capturing signals from the air, or a transmitter like a HackRF or ADALM-Pluto for signal transmission.  Each project folder contains a *.grc file, it's corresponding *.py file, a *.pdf file that shows the project flowgraph and a README.md file.  Some folders might contain several related projects, or supporting files for the project.  


#### Each project description below gives more details about what the project requires, as well as a brief explanation of what's going on.  See the README.md files in each folder for further details.  

#### We note the projects that don't require hardware are rather "naive" in the sense that issues that must be accounted for in real hardware systems: things like clock and timing recovery, phase and frequency misalignment, noise, signal amplitude variations, etc. are completely avoided.  These topics will be addressed in projects that use SDR hardware.  

#
#### Brief introduction
GNU Radio Companion uses a graphical user interface, very similar to Simulink or Labview, that allows the user to implement a variety of signal processing algorithms.  The user creates a "flow graph" by dragging-and-dropping blocks, and then connects them with wires.  Running the flow graph creates a Python script that actually implements the algorithm.  

#
#### References
Installing GNU Radio Companion: https://wiki.gnuradio.org/index.php/InstallingGR

About GNU Radio: https://wiki.gnuradio.org/index.php?title=Main_Page

About software-defined radio: https://en.wikipedia.org/wiki/Software-defined_radio

#
### Projects that don't require external hardware

#### ASK_Tx_simulator
"ASK_Tx_simulator" shows how to modulate a carrier with digital data using amplitude-shift keying (ASK).

#### DTMF_generator
The "DTMF_generator" project generates DTMF (Touch-Tone) signals, displays them in the time and frequency domains, and plays the Touch-Tones using the PC speaker. 

#### OOK_Tx_simulator
"OOK_Tx_simulator" shows how to modulate a carrier with digital data using on-off keying (OOK).     

#### OOK_Rx_simulator
"OOK_Rx_simulator" shows how to naively demodulate a carrier with digital data using on-off keying (OOK).   

#### OOK_decoder
"OOK_decoder" takes an IQ data file captured in the "OOK_capture" project and shows the signals in both time- and frequency domains.  No hardware needed as we use IQ data previously captured and stored in a file.

#### Signal_generator
Real and complex signals are generated and displayed in the time- and frequency domains.  

#
### Projects that require external hardware

#### OOK_capture
"OOK_capture" shows how to use an RTL-SDR dongle to display and capture OOK signals from a very old garage door opener.  You'll need a wireless key fob or garage door opener in addition to an SDR receiver for this project. 

#### FM_receiver_basic
"FM_receiver_basic" shows how to use an RTL-SDR dongle to demodulate and listen to a single, user-selected FM radio station using the PC speaker.  The user should know the frequency of the station they want to listen to.  
