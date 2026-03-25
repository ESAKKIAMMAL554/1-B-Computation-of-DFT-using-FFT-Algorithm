# EXPT 1b: Computation-of-DFT-using-FFT-ALGORITHM

## AIM
To perform and verify DFT using FFT-ALGORITHM by SCILAB.
## APPARATUS REQUIRED
PC installed with SCILAB
### DFT FFT-ALGORITHM
## PROGRAM
```
clear; 
clc; 
close; 
xn = [1 2 3 4 4 3 2 1] 
n1=0:1:length(xn)-1; 
subplot(2,2,1); 
plot2d3(n1,xn); 
xlabel('Time n'); 
ylabel('Amplitude'); 
title('Input Sequence'); 
Xk = fft(xn); 
K1=0:1:length(Xk)-1; 
magnitude=abs(Xk) 
subplot(2,2,2); 
plot2d3(K1,magnitude); 
xlabel('frequency(Hz)'); 
ylabel('magnitude(gain)'); 
title('magnitude spectrum'); 
angle = atan(imag(Xk),real(Xk)) 
subplot(2,2,3); 
plot2d3(K1,angle); 
xlabel('frequency(Hz)'); 
ylabel('Phase'); 
title('Phase spectrum') 
y= ifft(Xk) 
n2=0:1:length(y)-1; 
subplot(2,2,4) 
plot2d3(n2,y) 
xlabel('Time n'); 
ylabel('Amplitude'); 
title('Inverse FFT OF X(K)');
```
### CALCULATIONS:
<img width="1200" height="1600" alt="image" src="https://github.com/user-attachments/assets/cf117163-5200-43de-8913-f00049883ca2" />

### SAMPLE OUTPUT:


<img width="1600" height="1200" alt="image" src="https://github.com/user-attachments/assets/4e283609-da39-4527-9db5-8f7cd97b6a08" />


## RESULT:
Thus,  DFT using FFT-ALGORITHM for two given sequences were performed and its result was verified.

