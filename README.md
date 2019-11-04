# pruning_challenge


- Pruning is one of the methods for inference to efficiently produce models smaller in size, more memory-efficient, more power-efficient and faster at inference with minimal loss in accuracy, other such techniques being weight sharing and quantization.
- Although weight pruning can be a rather computationally expensive process compared to unit pruning, it is evident from the accuracy curves that overall weight pruning performs better than unit pruning.

- Since the inference time remains approximately the same for both pruning methods, it is possible to sacrifice training time to use weight pruning for a smaller, more efficient network.
- Sparse models are easier to compress, and sparsity allows us to store the weights much more efficiently. However, as we increase the sparsity and delete more of the network, the task performance will progressively degrade.
This is evident in the epoch and accuracy graphs, however in the case of unit pruning the degradation is more severe than weight pruning.
- Dropping a neuron affects the model performance greatly as we are effectively stopping the flow of information from flowing through and being processed. This is in contrast to weight pruning where setting a weight to 0 does not lead to as great of a loss as we are not dropping neurons -- so the values of the neurons stay the same even if we are setting weights to 0.
