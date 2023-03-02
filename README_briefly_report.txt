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