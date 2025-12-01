# Marvel Rivals FPS Analysis

<div align="center">

</div>

This are the visualizations for Marvel Rivals, starting from Season 4 to the present day. 

## Analysis with DLSS, Frame Generation Auto, Low-Mid Settings, Shaders compiled, and Smooth Motion Enabled)
<img width="1104" height="512" alt="Screenshot 2025-11-22 at 7 58 22 PM" src="https://github.com/user-attachments/assets/e0b6de6e-9e9c-4089-b308-66b71a0bac91" />

### Pearson Correlations: 
OVERVIEW: A value closer to 1 or -1 indicates a linear/strong correlation between two quantitative variables. If the value is 0, there is no correlation. 

Some of these should be self explanatory, such as GPU temp and GPU clock. The higher the GPU clock, the higher the temperature output. There are exceptions to this rule, but this is examining your everyday PC. 

1) **FPS vs GPU utilization:** 0.66
     - As GPU utilization starts to max out, so does our FPS. When utilization drops, so does FPS. But it's not a perfect correlation due to what happens on the screen. For example, a Dr. Strange portal in its entirety from formation to jumping through it can cause GPU utlization to spike to 100%, and drop FPS. In other games, this can be caused if too many dynamic graphics or events take place at once or upclose.
     - <img width="891" height="228" alt="Screenshot 2025-11-22 at 8 52 42 PM" src="https://github.com/user-attachments/assets/0335b35c-d215-4ab8-9ec7-8219bc90ccb7" />

3) **GPU Temp vs GPU Clock:** 0.79
     - This is self explanatory, so I won't include a graph as there are natural differences of 1-3°C (54-57°C) as the GPU hits and maintains its maximum clock speed at 2865 MHz for the majority of playtime. The only changes are the beginning of the game session, and the ending of the game session.
  
5) **FPS vs Render Latency:** 0.7
     - Render latency is defined as the amount of time it takes (in ms) for the GPU to render a single frame, from when the CPU sends it out to the GPU's completion of the task. Lower RL = Faster Response time. This is the whole premise of NVIDIA Reflex, which I forgot to include is enabled in all tests of Marvel Rivals.
  
     - It should be noted that FPS and Render Latency are not 1-of-1. FPS is overall what's on your screen, RL is measuring internally how long it takes one frame to run its course from the CPU to GPU and out to the screen. A high FPS (ex. 300 FPS) & high RL system (anything outside of 20ms) will have no competitive benefit if frames are being bottlenecked before being shown on screen. NVIDIA reports that anything from 5-20ms is excellent; this is dependent on a lot of factors from game and system.
     - <img width="827" height="412" alt="Screenshot 2025-11-22 at 9 54 02 PM" src="https://github.com/user-attachments/assets/17ceea8a-be76-4afd-ac14-f37cfb8d818b" />
  
7) **CPU Utilization vs GPU Utilization:** 0.51
     - <img width="1027" height="505" alt="Screenshot 2025-11-22 at 10 08 11 PM" src="https://github.com/user-attachments/assets/b187360c-121b-4d78-bdd5-bfb235bed444" />
    - Here we know that there is only a GPU bottleneck present during this gameplay, therefore Low-Medium settings is more than likely to be the maximum settings we can achieve. The GPU is maxed out and the CPU still has more than enough headroom to queue up the next frames and calculate what is happening on the screen if the GPU is not doing that. What surpises me here is how uniform the graph looks - the CPU trends like a polynomial. There is a weak correlation as GPU activity is not dependent on CPU activity; the outliers when the game starts and ends are what present this weak outlier.
