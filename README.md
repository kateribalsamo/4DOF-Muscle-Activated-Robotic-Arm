# 4DOF-Muscle-Activated-Robotic-Arm
Muscle-activated robotic arm that converts EMG bio-signals into real-time servo motor control using LabVIEW and NI DAQ hardware.

## Overview
This project demonstrates a muscle-activated robotic arm controlled using electromyography (EMG) signals captured through surface electrodes. The system translates human muscle activation into robotic joint movement by combining biomedical signal acquisition, analog signal conditioning, real-time data processing, and servo motor actuation.

EMG signals were amplified using an instrumentation amplifier and acquired through National Instruments DAQ hardware. A LabVIEW program was developed to continuously process incoming signals, extract activation levels using RMS and threshold-based filtering, and convert muscle activity into servo rotational angles using pulse width modulation (PWM). The project highlights the potential for non-invasive bio-signal control in assistive robotics and prosthetic device applications.

## Hardware and Software Implementation 
 The robotic arm was constructed using a modular metal bracket framework designed to replicate natural upper-limb motion. Servo motors were mounted at key joints to simulate elbow flexion, wrist flexion, and wrist rotation, allowing multi-axis movement. A pre-manufactured gripper was integrated as the end-effector to enable hand grasping and object manipulation. Surface EMG electrodes were used to capture voluntary muscle activation signals from the user. These signals were amplified using an instrumentation amplifier to increase signal amplitude and improve signal clarity before being transmitted to National Instruments DAQ hardware for data acquisition.
 
The control system was developed in LabVIEW using NI-DAQmx analog input configuration to continuously acquire EMG signals in real time. The software was organized into three primary loops: a user interface loop for acquisition control and waveform visualization, a DAQ loop for continuous signal collection, and a data processing loop that interpreted EMG signals and controlled robotic movement. RMS signal processing was used to quantify muscle activation levels, and threshold filtering was applied to remove noise and motion artifacts. Processed EMG signals were converted into servo rotational angles using pulse width modulation (PWM), mapping muscle activation intensity to joint movement and allowing smooth, responsive robotic control.

## Note 
Note: The LabVIEW source file can only be opened with LabVIEW software. A screenshot of the block diagram is included in the Media section to provide a visual overview of the program architecture.
