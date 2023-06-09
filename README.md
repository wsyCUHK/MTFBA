# MTFBA
The code will be release after the acceptance. Here, we first provide some extra simluation results, due to the page limit.

## SNR Performance
![SNR](./figures/SNR_VS_Codebook1214.png)
The goal of this paper is also to identify the candidate beam that achieves the highest SNR, as stated in Problem (8). We use the cross-entropy function to train the neural network, because the candidate codebook has made the SNR maximization decision variable discrete.

Here, we also plot the achieved SNR of the proposed approach and the baselines with increasing probing codebook size. The proposed method consistently outperforms Heng 2022 and the 2-Tier Hierarchical Search Method in terms of SNR as the number of measurements increases. Overall, MTFBA provide extra 3.1% (2.2%∼4.3%) average SNR compared with Heng2022. Furthermore, the advantage increases with the number of measurements.

## Ablation Study from the CDF perspective
![CDF](./figures/Ablation_FastBeamAlignment_CDFv4.png)
In this figure, we also evaluate the achieved SNR distribution across the channels in the testing dataset, to demonstrate how MTFBA improves the performance. When the network condition is poor or very good, all the methods achieve similar SNR. However, when the network condition is fair, the MTFBA selects better beams and enjoys higher SNR. Overall, the curve of MTFBA is in the bottom right corner, which means that MTFBA not only improves the average accuracy, but also improves the mean, lower quartile, median, and upper quartile of throughput. This shows that MTFBA achieves high SNR under various channel conditions.
