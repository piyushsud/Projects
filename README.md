# Projects
This engineering portfolio contains some of the engineering projects I have worked on. 

1. UIUC Senior Design Project - a house for mason bees with capacitive sensors to detect when bees enter and exit. We used phase sensitive detection to extract the bee data in a noisy environment.
<img width="655" height="873" alt="image" src="https://github.com/user-attachments/assets/4252c7ad-c963-4968-b640-8132281498dd" />

2. FM Radio Receiver - I built this as a learning project on a PCB. See my linkedin page for a video demo!
<img width="1255" height="945" alt="image" src="https://github.com/user-attachments/assets/bec27199-4515-4227-bf64-04a886c5d29d" />

3. Sample and Hold Test PCB - I built this for my research lab at USC. Another group at USC designed a custom 64 channel interleaved sample and hold IC, to sample and hold a sine wave at 640 MHz and output all channels at 10 MHz. I designed this PCB to interface with that sample and hold IC by providing the clock and input signals, and sending the output to a CAEN DT2740 64-channel high speed digitizer.
<img width="853" height="764" alt="image" src="https://github.com/user-attachments/assets/948636f7-ad70-458c-a41c-5e8fa63eacdf" />


The project which I am the most proud of is an FM radio receiver. 

<img width="1065" height="302" alt="image" src="https://github.com/user-attachments/assets/f709599a-ae21-4d2b-a37c-8b03bd871731" />

I have assembled the PCB and tested it at home - a short video is on my LinkedIn page. I've taken detailed notes on my design process, tradeoffs, part selection, and more in this repo: https://github.com/piyushsud/knowledge/tree/master

The design for each stage in the radio is a LaTex PDF under the respective folder for each stage, under knowledge/Project_Specific_Knowledge/public/fm_radio/stages. I've also put some less organized notes in the brain dump folder.  

Note that my design has the following errors, which I discovered during board bringup:

1. The input filter does not match 75 ohms to 50 ohms => I used a filter design tool that allows you to specify the input and output impedances, but doesn’t actually integrate a matching network into the filter. 
2. The PLL voltage level for all digital interfaces is 1.9V, but I used 3.3V. 
3. I did not include a bypass cap for the LM386 near the power supply.

If you have any questions, feel free to reach out at piyushsud@gmail.com!.

Input stage:

<img width="1091" height="341" alt="image" src="https://github.com/user-attachments/assets/1d75897a-50b2-4e82-97ef-9cc0880493ca" />

HF amp:

<img width="806" height="535" alt="HF_amp_circuit" src="https://github.com/user-attachments/assets/9f8fc01b-58bd-48f6-ab23-948bd8e23b61" />

Mixer:

<img width="901" height="401" alt="mixer_circuit" src="https://github.com/user-attachments/assets/ede03d80-5c75-49e3-93fb-0c9f4aaebaaf" />

Local Oscillator:

<img width="1053" height="700" alt="LO_circuit_final" src="https://github.com/user-attachments/assets/d2dcd61c-7cdc-4645-8af0-a4814349c11f" />

Variable gain amp:

<img width="1102" height="841" alt="variable_gain_amp_circuit" src="https://github.com/user-attachments/assets/2daea12b-6ca9-460e-88ef-ae0e6fe3acb7" />

FM detector:

<img width="1200" height="682" alt="fm_detector_circuit" src="https://github.com/user-attachments/assets/1ea7fd3e-f01b-4ee4-9edd-388a8ffceac7" />

Output stage:

<img width="1225" height="546" alt="image" src="https://github.com/user-attachments/assets/9952dd2d-f81c-4a3c-870d-179bc2cb7f05" />

Power:

<img width="878" height="843" alt="power_circuit" src="https://github.com/user-attachments/assets/90fd8417-b41b-4a36-a75e-df192e734be1" />







