### EXPT 1b: Computation-of-DFT-using-FFT-ALGORITHM

### AIM
To perform and verify DFT using FFT-ALGORITHM by SCILAB.
### APPARATUS REQUIRED
PC installed with SCILAB
### PROGRAM 
### DFT FFT-ALGORITHM
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
<img width="1291" height="1291" alt="WhatsApp Image 2026-08-25 at 12 34 09" src="https://github.com/user-attachments/assets/afa7b249-77cf-4090-9894-69446f148333" />
<img width="1008" height="1008" alt="WhatsApp Image 2026-08-25 at 12 34 45" src="https://github.com/user-attachments/assets/3245dee2-d033-4831-b766-1f0c8bc82114" />
<img width="952" height="952" alt="WhatsApp Image 2026-08-25 at 12 35 26" src="https://github.com/user-attachments/assets/674f0f80-da39-4665-8e5f-76abd31c393a" />

### SAMPLE OUTPUT:
<img width="755" height="591" alt="Screenshot 2026-07-27 221059" src="https://github.com/user-attachments/assets/c119dcaf-7d16-4557-83cc-055a9d46e937" />




## RESULT:
Thus,  DFT using FFT-ALGORITHM for two given sequences were performed and its result was verified.

