# Matlab signal processing  
## read the signal from files  
ecg_sig = load('ecg.txt')  
plot(ecg_sig)  
ylabel('Amplitude')  
xlabel("Sample Number")  
![image](https://user-images.githubusercontent.com/88282118/191026039-d7b71a29-99fb-4a42-bbfc-fa4452830790.png)  
len_ecg = length(ecg_sig);  
save('ecg_data.mat', 'ecg_sig', 'len_ecg');  
clear all; %clear all variables from the workspace.  
whos %show that there are no variables  
load('ecg_data.mat') % load the variables back in  
whos % show that the variables have been reloaded  
![image](https://user-images.githubusercontent.com/88282118/191027942-20ed2600-a617-454b-a945-002b4121f4b0.png)  
[sound_sig fs] = audioread('C:\Users\Shilelon\Desktop\Matlab\drums.wav');  % fs is the frequency of simple  
sound(sound, fs);  % play the audio  
image_signal = imread('Winter.jpg');  
image(image_signal);  
![image](https://user-images.githubusercontent.com/88282118/191035351-bcfff663-796a-48ee-a908-314d49ea40e8.png)  
