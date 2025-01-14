#my-work #system-overview

Although our wider system design (shown in Figure 1) incorporates a diverse set of signals acquired from both performers and the audience, for the purposes of this paper we focus on an ECG subsystem that we primarily worked with in our preliminary visit (shown in yellow in Figure 1). Functioning as a proof-of-concept, this subsystem (shown in Figure 2) is fundamentally based upon the acquisition of an ECG signal from a performer, from which the temporal positions of the R-peaks are extracted in real-time. The identification of an R-peak triggers a brief double flash of red background LED, to signify a heart beat and convey a sense of the performer's heart rate.


![[Aarhus_System_ECG.png]]
Figure 1 - A high level overview of our system to map a diverse set of signals acquired from both performers and the audience to the concert house lighting system. For the purposes of this paper, we focus on the preliminary work done with the performer ECG signals, with the signal chain shown highlighted in yellow.

# R-Peak Extraction

 In ECG signals, a single heart beat is represented through a series of five deflections from the zero-voltage line termed a PQRST complex (Figure 3). These correspond to atrial depolarisation, three phases of ventrical depolarisation, and ventrical repolarisation respectively [ref]. The R-wave deflection is the most prominent of these, and the temporal location of its peak is commonly used to calculate higher order features such as the heart rate and heart rate variability. Although many algorithm exist to extract the QRS complex representing ventrical polarisation, we employ the Pan-Tompkins algorithm 