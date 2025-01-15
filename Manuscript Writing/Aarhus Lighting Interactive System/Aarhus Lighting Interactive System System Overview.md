#my-work #system-overview

Although our wider system design (shown in Figure 1) incorporates a diverse set of signals acquired from both performers and the audience, for the purposes of this paper we focus on an ECG subsystem that we primarily worked with in our preliminary visit (shown in yellow in Figure 1). Functioning as a proof-of-concept, this subsystem (shown in Figure 2) is fundamentally based upon the acquisition of an ECG signal from a performer, from which the temporal positions of the R-peaks are extracted in real-time. <span style="background:#ff4d4f">The identification of an R-peak triggers a brief double flash of red background LED, to signify a heart beat and convey a sense of the performer's heart rate.</span>


![[Aarhus_System_ECG.png]]
Figure 1 - A high level overview of our system to map a diverse set of signals acquired from both performers and the audience to the concert house lighting system. For the purposes of this paper, we focus on the preliminary work done with the performer ECG signals, with the signal chain shown highlighted in yellow.

# R-Peak Extraction

 In ECG signals, a single heart beat is represented through a series of five deflections from the zero-voltage line termed a PQRST complex (Figure 3). These correspond to atrial depolarisation, three phases of ventrical depolarisation, and ventrical repolarisation respectively [ref]. The R-wave deflection is the most prominent of these, and the temporal location of its peak is commonly used to calculate higher order features such as the heart rate (time difference between two R-peaks) and heart rate variability (change in time difference between two R-peaks). Although many algorithm exist to detect the QRS complex representing ventrical polarisation, we employ the commonly used Pan-Tompkins algorithm [ref] to extract the temporal position of the peak of the R-wave within the ECG signal buffer. This involves a series of a bandpass filter, a derivative filter, a squaring filter, and a moving average filter. 
# Mapping

TBD

# Implementation

We acquire the ECG signal from six performers using two BioArmbands and four BioPoints. Similar to a Myo, the BioArmband  (Figure 4) is multi-sensor device is worn around the forearm. It contains an eight-channel EMG, an ECG, an six-axis IMU, a GSR, and a PPG sensor. A lead can be connected to enable the attachment of an ECG pad to create a second contact point across the heart. The BioPoint (Figure 5) is identical, with the exception that it contains only a single channel EMG and must be attached with a velcro band.

The ECG signal is collected at 500Hz and transported to a laptop via a Bluetooth connection in packets of eight samples. Within Max, the ECG signal is fed into a two second first-in-first-out buffer, and we extract the R-peak position using a self-implemented Max object which calculates the heart-rate from an ECG signal.[^1] Lighting parameters are sent over OSC to the GrandMA3 lighting desk installed in the concert hall.
# Footnotes

[^1]: Link here