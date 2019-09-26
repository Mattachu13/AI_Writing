# AI Writing
Experiments in AI writing using TensorFlow  

## Raspberry Pi 3B

### Summary

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

### Notes on Tensorflow installation
Tensorflow should be installed with `pip install --no-cache-dir tensorflow`
* If this fails, install the following dependencies independently:
  * `setuptools, termcolor, enum34, six, absl-py, numpy, h5py, keras-applications, futures, grpcio, keras-preprocessing, funcsigs, pbr, mock, gast, protobuf, markdown, werkzeug, wheel, tensorboard, backports.weakref, astor, tensorflow`
  * `h5py` requires `sudo apt-get install libhdf5-dev`
  * If any of these cause issues, try `pip install --no-cache-dir --no-deps`

## Ubuntu for Windows 10

Successful test with Alice's Adventures in Wonderland + Through the Looking-Glass

Test on The Count of Monte Cristo, but be aware of hardware; even on the test run above,
the computer became very loud and CPU usage hit 100%

### Notes on Tensorflow installation

* (Install Python if required)
* `sudo apt install python-pip`
* `pip install tensorflow`
* `wget https://github.com/hunkim/word-rnn-tensorflow/archive/master.zip`
