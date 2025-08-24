# NVIDIA FPS Analysis
The NVIDIA app now allows for stats tracking for all things FPS and GPU! One of the biggest features is now tracking what DLSS does in terms of Frame Gen, Super Resolution, and Smooth Motion. Analysis will be run here. Hopefully no code. 

# Specs
All tests are run on my personal computer, a Ryzen 5 5500 and RTX 4060 with 32 GB of RAM. The 4060 and RAM are overclocked to 2603MHz and 3200MT/s respectively.

# Patch Notes (Version 11.0.5.238)

Paired with a new Geforce Game Ready Driver (581.08) that came with an update to the app, this brings to the table:

* DLSS Override global toggle (for every *compatible* game on your system)
    * **DLSS Multi FrameG Override**: RTX 50 series owners can have this with FG enabled in game for titles without native DLSSMFG support.
    * **DLSS Frame Generation Model Upgrade**: RTX 40 AND 50 series users can have FG on, AND see reductions in VRAM usage while having an increase in FPS.
    * **DLSS Transformer Model Upgrade**: Enables NVIDIA's latest transformer model for DLSS Super Resolution, Ray Reconstruction, and DLAA for ALL RTX users (with FG on).
    * **DLAA & Ultra Performance Modes**: NVIDIA app now has internal solutions for DLSS Super Resolution, enabling DLAA or Ultra Performance in games without this native support (needs Super Resoultion ON in-game). This is customizable.
* Smooth Motion (now available to the RTX 40 series)
    * Smooth Motion comes with the latest NVIDIA driver. It is an AI model that inferences from two rendered frames to inject a generated frame in between to create smoother gameplay. This should be used in games without native DLSS support.
* Merging of some Control Panel features
* Removed limitations of Project G-Assist (now all RTX cards upwards of 6GB VRAM can use it)
* Streamlined NVIDIA Surround Setup

# Purpose of this Repository
This is simply personal use, but if it benefits you that's all the better for all of us. I will be playing games, and uploading the output from the NVIDIA app, which will be in a Excel file. I will analyze these data points in addition to listing what settings were in the game at the time, and run it from multiple perspectives.
If it somehow requires it, I will upload code as well. NVIDIA did say this was a beta feature still.

# Example Findings
**Marvel Rivals**:
   * No DLSS, but high settings (**with shaders compiling**): 54.92 FPS Average
   * DLSS, Frame Gen Auto, high settings, shaders compiled: 115.14 FPS Average
   * DLSS, Frame Gen Auto, Mid-to-Low textures, shaders compiled, and Smooth Motion active (**overclocks applied**): 236.08 FPS Average

**Stellar Blade**:
   * DLSS 4, medium settings, shaders compiled, Smooth Motion active, no frame generation: 192.67 FPS average

**Death Stranding**:
   * DLSS Quality, No Frame Generation, shaders compiled, high settings, Smooth Motion enabled: 147.63 FPS average

# Candidates for Generated Frames
<img width="1440" height="809" alt="Screenshot 2025-08-23 at 8 48 10 PM" src="https://github.com/user-attachments/assets/8b5813cd-ad31-4817-90d6-8df8908c66b4" />
<img width="1440" height="811" alt="Screenshot 2025-08-23 at 8 46 29 PM" src="https://github.com/user-attachments/assets/93354b1f-7bb5-43e4-9294-d6daf634deb3" />
<img width="1435" height="812" alt="Screenshot 2025-08-23 at 8 41 35 PM" src="https://github.com/user-attachments/assets/f08e0fcd-30de-49d8-8716-47b938c1b9aa" />
<img width="1440" height="809" alt="Screenshot 2025-08-23 at 8 40 33 PM" src="https://github.com/user-attachments/assets/61d2345a-0b70-4cb6-9196-fc8270a02c06" />
<img width="1439" height="811" alt="Screenshot 2025-08-23 at 8 34 01 PM" src="https://github.com/user-attachments/assets/fe2bf5c4-cd66-483b-ab37-9cd724c6f285" />
<img width="1440" height="809" alt="Screenshot 2025-08-23 at 8 33 51 PM" src="https://github.com/user-attachments/assets/1a60718c-bdf2-4d7b-bbc1-b520513f87f7" />
<img width="1438" height="810" alt="Screenshot 2025-08-23 at 8 33 37 PM" src="https://github.com/user-attachments/assets/a25ecfed-1e9b-47cd-81de-8a1cdcb0596f" />
<img width="1440" height="810" alt="Screenshot 2025-08-23 at 8 33 25 PM" src="https://github.com/user-attachments/assets/d1b95b58-ddf0-4578-8762-01c31a9cde8e" />
<img width="1440" height="808" alt="Screenshot 2025-08-23 at 8 00 09 PM" src="https://github.com/user-attachments/assets/403c502e-e6ff-4074-9751-500d59d03c29" />


