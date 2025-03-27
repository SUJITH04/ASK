### EXPT   NO 1	:		SIMULATION OF AMPLITUDE SHIFT KEYING
### DATE		: 

### AIM : To implement ASK using MATLAB.

### SOFTWARE REQUIRED : MATLAB
### PROGRAM:

AMPLITUDE SHIFT KEYING
'''
clc; 
clear all; 
close all;
fc=input('Enter the freq of Sine Wave carrier:');
fp=input('Enter the freq of Periodic Binary pulse (Message):');
amp=input('Enter the amplitude (For Carrier & Binary Pulse Message):');
t=0:0.001:1; % For setting the sampling interval
c=amp.*sin(2*pi*fc*t);% For Generating Carrier Sine wave
subplot(3,1,1) %For Plotting The Carrier wave
plot(t,c)
xlabel('Time')
ylabel('Amplitude')
title('Carrier Wave')
m=amp/2.*square(2*pi*fp*t)+(amp/2);%For Generating Square wave message
subplot(3,1,2) %For Plotting The Square Binary Pulse (Message)
plot(t,m)
xlabel('Time')
ylabel('Amplitude')
title('Binary Message Pulses')
w=c.*m; % The Shift Keyed Wave
subplot(3,1,3) %For Plotting The Amplitude Shift Keyed Wave
plot(t,w)
xlabel('Time')
ylabel('Amplitude')
title('Amplitide Shift Keyed Signal')
'''




INPUTS GIVEN TO GENERATE ASK MODULATED WAVE:
Enter the freq of Sine Wave carrier:100
Enter the freq of Periodic Binary pulse (Message):10
Enter the amplitude (For Both Carrier & Binary Pulse Message):4




### OUTPUT

![Adc 01](https://github.com/user-attachments/assets/1af7cdcf-e837-48e7-8538-6af02545dc50)






### RESULT
	Thus the generation of ASK was implemented using MATLAB.
