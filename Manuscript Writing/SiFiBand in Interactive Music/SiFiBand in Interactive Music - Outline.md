#my-work 


# Introduction

Introduce context for IMU/EMG portable systems in interactive music and research contexts. Explain that Myo used a lot, but that is no out of production. Frame SiFiBand as lineage with Myo. It is also important to evaluate the relationship between the two devices while it is still possible (Myos aren't all dead)

# Background and Related Work

Short review of works using EMG/IMU in interactive music performance and research, especially those using Myo.

# Methods

Three categories of devices:

1. Myo
2. SiFiBand
3. Qualisys/Delsys

Three broad categories of evaluation:

## Technical Evaluation

1. Latency
2. Jitter
3. Noise

Use Qualisys and Delsys as measurement tools for IMU and EMG.

## Interactive Music Based Tasks

We fill follow a framework of sound-action typologies. One impulsive action, one iterative action and one sustained action.

1. Impulsive - Hit a snare drum with a drumstick
2. Iterative - Repeatedly run a scale on a piano
3. Sustained - Bowing on saw

We will create a simple sonification for each of these. We will also collect the motion and EMG from Qualisys and Delsys as reference signals.

### Evaluation Metrics

1. Analysis of signal similarities in EMG and IMU
2. Analysis of audio signal similarities between generated audio from mapping SiFiBand and Myo
3. Train a basic gesture recognition ML model mapping (use Wekinator and PD) and evaluate ability to recognise gestures, one regression model (mapped to synth param), one classification model (mapped to toggle on/off)
4. Latency between EMG peak and IMU peak