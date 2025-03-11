#my-work 

# General Set-Up

Attach three markers to SiFiBand and Myo. Define each as a rigid body within Qualisys.

Prepare a Python Script which receives OSC packets from Qualisys of both EMG (Delsys), IMU (Delsys) and MoCap, Bluetooth packets of EMG and IMU from SiFiBand, and EMG and IMU from Myo. Each receiver runs on a separate thread and appends a timestamp upon the reception of each packet.

![[BA_Setup.png]]
# Technical Evaluation

## Latency and Jitter

Latency of SiFiBand and Myo are measured relative to Delsys and Qualisys.
### Set-Up

Modify script to add a timecode log upon packet request for Myo and SiFiBand.

### Conditions

Two conditions will be tested:

- Distance from logging computer: 0m, 2m, 5m
- Sensors Activated: IMU, EMG, IMU and EMG

### Procedure

For each device and combination of conditions, the device will be worn on the forearm and data logged for five minutes. Here, there is no need to use Qualisys and Delysis as references.

## Noise

Following MuMyo paper:

#### IMU

##### Set Up
Set SiFiBand and Myo on floor.

##### Procedure
Log SiFiBand, Myo, Qualisys for five minutes.

### EMG

##### Set Up
Test the 8 SiFiBand, 8 Myo, and Delsys separately.

Place each sensor in the same position on the belly of the extensor digitorum. Mark the position with a pen.
##### Conditions

Each sensor will be logged twice for two conditions: at rest and full effort finger extension. At rest means with the arm resting on the arm of a chair with no active muscle activity. Full effort finger extension means resting the arm on the arm of a chair and fully extending all fingers.
##### Procedure

Log each condition for 30 seconds.

# Music Based Tasks

## Impulsive 

Hitting a snare drum

## Procedure

Log each of the devices (SiFiBand, Myo, Delsys) separately.



