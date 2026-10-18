# Radar Signal Processing - Automotive - Radar - Distance and Speed Estimation - Interference Analysis [with MATLAB Code]

Main objectives
Impact Analysis: The study investigates how FMCW radar jamming affects target detection accuracy, particularly how it impacts the measurement of distance and velocity of nearby objects.
Data-Driven Insights: Analyze and visualize how interference disrupts the ability of radar to accurately detect and track targets using collected data.
Filter implementation: Test and demonstrate the effectiveness of various filtering technologies aimed at mitigating the negative impacts of radar interference, thereby enhancing radar performance and reliability.
Data Explanation
The dataset includes parameters from both interfered radar systems and interfered radar systems:
Victim radar parameters:
EIRP: -5 dB
Antenna gain: 10 dBi
Starting frequency: 76.5 GHz
Bandwidth: 500 MHz
Scan time: 50 μs
Pulse repetition interval: 60 μs
Coherent processing interval: 10 ms
Low-pass filter cutoff frequency: 3.5 MHz
Signal modulation: FMCW
Antenna configuration: Single-node (initial), TDMA-MIMO (advanced stage)
Speed: (0, 0) m/s
Interference radar parameters:
EIRP: -5 dB
Starting frequency: 76.45 GHz
Bandwidth: 900 MHz
Scan time: 25 μs
Pulse repetition interval: 30 μs
Signal modulation: FMCW
Objective:
Objective 1: Dimensions (4 m x 1.9 m x 1.5 m), speed (10, 0) m/s, position (40, 3.6) m
Objective 2: Dimensions (4.5m x 1.9m x 1.5m), speed (-5,0) m/s, position (20,7.2) m
MATLAB code
MATLAB scripts to process radar data to analyze the impact of interference and evaluate different filtering techniques. This code calculates the radar signal properties. Handle signal interference. And generate outputs demonstrating the effects of various filters.
MATLABCodeclear all;\nclc;\n% Victim radar parameters\nfc = 76.5e9; % Start frequency\nbw_sv = 500e6; % Bandwidth\ntm_sv = 50e-6; % Sweep time\nfs_sv = bw_sv; % Sampling frequency\nN_sv = 25000; % Number of samples in each chirp\nNd_sv = 135; % Number of chirps\n% Initialize variables for later use\nN=N_sv;\nNd=Nd_sv;\nfs=fs_sv;\nc=3e8;\nslope=bw_sv/tm_sv; % Frequency slope\nlambda = c/fc; % Wavelength (m)\ntm=tm_sv;\n% Interferer radar parameters\nfc_int = 76.45e9; % Start frequency\nbw_int = 900e6; % Bandwidth\ntm_int = 25e-6; % Sweep time\nfs_int = bw_int; % Sampling frequency (Hz)\n% Time vectors\nt_sv = 0:1/fs_sv:(tm_sv*Nd_sv)-1/fs_sv; % Victim radar\n\n  

## Images

![(Radar Signal Processing)Automotive - Radar - Distance and Speed Estimation - Interference Analysis [with MATLAB Code]](01.jpg)
![(Radar Signal Processing)Automotive - Radar - Distance and Speed Estimation - Interference Analysis [with MATLAB Code]](02.jpg)

<!-- PAYMENT_BLOCK -->

## Get this dataset

- Payment link (Stripe): [Buy now](https://buy.stripe.com/3cs8yP7sY87d0vu9AB)
- Payment QR code: ![Payment QR code](pay.png)

<!-- /PAYMENT_BLOCK -->
