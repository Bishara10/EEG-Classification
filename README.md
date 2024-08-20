# ML Classification model for EEG Recordings
A ML classification model for classifying patients as ADHD or no ADHD based on their EEG recordings 

Dataset reference:
Ali Motie Nasrabadi, Armin Allahverdy, Mehdi Samavati, Mohammad Reza Mohammadi, June 10, 2020, "EEG data for ADHD / Control children", IEEE Dataport, [more information here](https://ieee-dataport.org/open-access/eeg-data-adhd-control-children)

## Abstract [more information](https://ieee-dataport.org/open-access/eeg-data-adhd-control-children)
Participants were 61 children with ADHD and 60 healthy controls (boys and girls, ages 7-12). The ADHD children were diagnosed by an experienced psychiatrist to DSM-IV criteria, and have taken Ritalin for up to 6 months. None of the children in the control group had a history of psychiatric disorders, epilepsy, or any report of high-risk behaviors.

EEG recording was performed based on 10-20 standard by 19 channels (Fz, Cz, Pz, C3, T3, C4, T4, Fp1, Fp2, F3, F4, F7, F8, P3, P4, T5, T6, O1, O2) at 128 Hz sampling frequency. The A1 and A2 electrodes were the references located on earlobes. 

## Implementation
### Preprocessing
Dataset was preprocessed by applying BandPass filter for noise reduction in signal recordings for each channel.

### Feature extraction
Calculated Pearson correlation between every two channels for every patient.

### Machine Learning model
Utilized SVM model for classifying recordings as ADHD / Non-ADHD


## Results
Achieved 85% accuracy. However, the test was done on 10% of the dataset, considering the relatively small amount of patients.
![image](https://github.com/user-attachments/assets/fc1ef355-a2a7-4241-aaaa-47a44bfe9683)
