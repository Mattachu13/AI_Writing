# AI Writing
Experiments in AI writing using TensorFlow  
Performed using Raspberry Pi 3B

## Summary

| Test |                         Training set                         | Training set size | Output size |    Results     |
|------|--------------------------------------------------------------|-------------------|-------------|----------------|
|  1   | Chapter 1 of Alice's Adventures in Wonderland                |       2,140 words |   500 words | Incoherent     |
|  2   | Alice's Adventures in Wonderland                             |      26,449 words | 1,500 words | Incoherent     |
|  3   | Alice's Adventures in Wonderland + Through the Looking-Glass |      55,741 words | 1,500 words | Rare coherence |

Tutorial: https://medium.com/deep-writing/how-to-write-with-artificial-intelligence-45747ed073c
* This tutorial is intended for Mac, so TensorFlow should be installed using the [instructions on the homepage](https://www.tensorflow.org/install/install_raspbian)

Important note: Due to freezing caused by suspected excessive power draw, these tasks were run via SSH, with HDMI and USB bluetooth mouse disconnected to minimise
power requirements.

Investigate: Possibility of resuming failed jobs
