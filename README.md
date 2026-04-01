# Digital-Signal-Processing--Convolution
## Aim:
                  To perform linear convolution using MAT LAB.
## Software Required:
MAT LAB R2012
## Algorithm:
Step 1: Open mat lab. Write the program.

Step 2: Read the first input sequence.

Step 3: Read the second impulse sequence.

Step 4: Plot the input sequences with x-label and y-label with suitable title. 

Step 5: Perform convolution for both the sequences using conv2() function.
  
Step 6: Plot the sequence with x-label and y-label with suitable title

Step 7: Terminate the program.

## PROGRAM: 
```
clc;%clear screen
clear all;%clear screen
close all;%close all figure windows

%INPUT SEQUENCE
%x[n]={2,−2.3,5,−1,4,9,−3}
%h[n]={3, −2.3,2.7,3.5,2,5 − 4,1,1}
a=input('enter the starting x(n)');
x=input('enter the x(n) sequence');
n=a:1:length(x)+a-1;
figure(1);
stem(n,x);
xlabel('time');
ylabel('amplitude');
title('input sequence');

%IMPULSE SEQUENCE
b=input('enter the starting h(n)');
y=input('enter the h(n) sequence');
m=b:1:length(y)+b-1;
figure(2);
stem(m,y);
xlabel('time');
ylabel('amplitude');
title('impulse response');

% LINEAR CONVOLUTION
z=conv2(x,y);
n1=a+b:1:length(z)+a+b-1;
figure(3);
stem(n1,z);
xlabel('time');
ylabel('amplitude');
title('linear convolution');
```

## OUTPUT:
### Input Sequence:

<img width="697" height="378" alt="image" src="https://github.com/user-attachments/assets/0821b9e2-5491-470e-bfeb-1958b3111783" />



### Impulse Sequence:

<img width="690" height="411" alt="image" src="https://github.com/user-attachments/assets/36df8cdb-caa4-4b80-bc79-91175eb94015" />


### Linear Convolution:

<img width="696" height="474" alt="image" src="https://github.com/user-attachments/assets/0e717e81-3b67-4bdc-b48a-334885f4c025" />




## RESULT:
![WhatsApp Image 2026-04-01 at 23 17 28](https://github.com/user-attachments/assets/af02c5e8-8672-4ce3-9431-0f758f30b4fe)


