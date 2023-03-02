# Alpha-rhythm-of-EEG
Analysis of the alpha rhythm of EEG

A program has been developed in the MATLAB “App Designer” utility that allows filtering the EEG signal, 
plotting the original signals, filtered signals, their autocorrelation function and spectral power density. 
For SPD, a modified covariance method was used.

A model of a band-pass FIR filter was developed, with a standard deviation minimization of 22 orders with transmission 
frequencies from 8 Hz to 13 Hz, which corresponds to the frequencies of the alpha rhythm in the EEG signal.
 
According to the obtained map of zeros and poles, the filter is stable. The frequency response of the bandpass filter 
is not very smooth, which can cause non-linear distortion of the passband signal. The impulse response 
coefficients are the same as the filter coefficients, which is characteristic of FIR filters.

The Welch method was used to estimate the SPD with segment sizes: 100,200,500; 70% overlap and Hamming window 
(set by default when using the pwelch method)

The given signal was digitally processed.

# Filter designing 
![1](https://user-images.githubusercontent.com/90864757/222421389-7a0a65ec-9e3f-4f5d-992b-c3ea4728d01a.png)

# The app window with downloaded signal
![2](https://user-images.githubusercontent.com/90864757/222421866-a21e0e6c-82dc-4751-b5ad-3179b44be13a.gif)
