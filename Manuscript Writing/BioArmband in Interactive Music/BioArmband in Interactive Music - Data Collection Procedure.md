#my-work 

# General Set-Up

Prepare a Python Script which receives OSC packets from Qualisys of both EMG (Delsys) and MoCap, Bluetooth packets of EMG and IMU from BioArmband, and EMG and IMU from Myo. Each receiver runs on a separate thread and appends a timestamp upon the reception of each packet.

![[BA_Setup.png]]
# Technical Evaluation

## Latency and Jitter

Latency of BioArmband and Myo are measured relative to Delsys and Qualisys.
### Set-Up

Attach three markers to BioArmband and Myo. Define each as a rigid body within Qualisys.

### Conditions

Distance from computer