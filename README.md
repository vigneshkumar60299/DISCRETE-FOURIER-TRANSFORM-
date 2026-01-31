# EXP 1 A : COMPUTATION OF DFT USING DIRECT AND FFT

# AIM: 

# To Obtain DFT and FFT of a given sequence in SCILAB. 

# APPARATUS REQUIRED: 
PC installed with SCILAB. 

# PROGRAM: 
// DISCRETE FOURIER TRANSFORM
```
clc;
clear;
xn = [1 1 1 1 0 0 0 0];
n1 = 0:1:length(xn)-1;
subplot(3,1,1);
plot2d3(n1, xn);
xlabel('Time n');
ylabel('Amplitude xn');
title('Input Sequence');
Xk = fft(xn);
disp(Xk);
K1 = 0:1:length(Xk)-1;
magnitude = abs(Xk);
subplot(3,1,2);
plot2d3(K1, magnitude);
xlabel('Frequency index k');
ylabel('Magnitude');
title('Magnitude Spectrum');

phase = atan(imag(Xk), real(Xk));
subplot(3,1,3);
plot2d3(K1, phase);
xlabel('Frequency index k');
ylabel('Phase');
title('Phase Spectrum');

```


# OUTPUT: 
<img width="1915" height="945" alt="Screenshot 2026-01-31 113653" src="https://github.com/user-attachments/assets/405d3fd0-216b-42d1-a51f-f106aea40c03" />




# RESULT: 
