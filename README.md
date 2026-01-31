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

xn = [1 2 3 4 4 3 2 1];
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
<img width="1919" height="1028" alt="Screenshot 2026-01-31 113348" src="https://github.com/user-attachments/assets/f2aba7ca-fbf8-44c1-810e-3ab123ef152f" />



# RESULT: 
