# GRCProjects
MyGRCCode
GRC projects from the ground up

Developed and tested using GNU Radio Companion 3.10.1.1 on a Linux system using Ubuntu 22.04.2 LTS

Each folder contains a project with a *.grc file, a corresponding *.py file, and a *.pdf file that shows the project blocks layout. The only file one really needs is the *.grc file.

The "DTMF_generator" project generates DTMF (Touch-Tone) signals, displays them in the time and frequency domains, and plays the Touch-Tones using the PC speaker. No external hardware required. This flowgraph is just a gentle introduction to GNU Radio Companion basics.

"OOK_capture" shows how to use an RTL-SDR dongle to display OOK signals from a garage door opener, in this case one having a carrier frequency of approximately 390 MHz. The user should set the appropriate frequency for their device (it's usually written on the device somewhere), and don't forget to use an antenna with the SDR dongle. The time and frequency domain OOK signals are shown, along with the constellation plot, which is pretty simple in this case. We also compute the magnitude of the complex time domain signal, decimate it, and show it in the time domain - allowing us to clearly see the 0's and 1's that were transmitted. The decimated signal is also sent to an audio sink - the PC speaker - so we can hear the bursts generated when the garage door opener button is pushed.
