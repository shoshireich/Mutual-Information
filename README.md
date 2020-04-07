# Mutual-Information
## Abstract
In the paper "Using deep sequencing to characterize the biophysical mechanism of a transcriptional regulatory sequence" by Kinney et. al., the authors look at nucleotide positions that affect expression in order to locate functional binding sites within a promoter. They use an information footprint to determine which binding site is involved in response to specific biochemical signals. The information footprint is created using mutual information. The method described in the paper are repeated using the same publically-available dataset in order to replicate the information footprint.

## Methods
The data from Kinney et. al.'s full-wt experiment is a set of 75 base-pair-long (bp) sequences and a batch number indicating the fluorescence level (0-9) of the bacteria with that sequence. For each nucleotide position, the number of sequences in each batch μ having each of the four possible bases b_i (A, C, T, or G) is determined. The mutual information between batch and base is calculated for each nucleotide position. 

## Results and Discussion
All of the mutual information from each nucleotide position creates an information footprint. This recreation appears to be nearly identical to the footprint created by the original authors. The footprint can be used to determine which site is involved in response to specific biochemical signals. For the specific lac promoter examined in this study, two of the known sites are within nucleotide positions [-72:-51] with a six-pt gap between them. The other two known sites are at nucleotide positions [-41:-35] and [-10:-1]. This corresponds to the increased mutual information at these locations, as seen in the figure below. 

<img src="https://github.com/shoshireich/Mutual-Information/blob/master/Images/Replication.png" width="60%">
