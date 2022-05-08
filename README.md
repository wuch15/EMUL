# EMUL
source code for "Inference-efficient Machine Unlearning via Model Knowledge Assembling"

## Main Dependencies
* numpy
* Keras>=2.2.4
* tensorflow>=1.12.0

## Hardware requirements
For small dataset such as Adult, GPU is not mandatory but still recommended.

## Training and Testing
* The datasets need to be downloaded it from the original official sites. The model training is first conducted on each data shard (the total time can be similar to learning from scratch on the full data). When a data point is deleted, one model is retrained and the knowledge assembling part is also updated. The final single model is used for test.
