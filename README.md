# NVIDIA
INFO about NVIDIA GPUs

# NVIDIA TESLA WORKSTATION GPU PERFORMANCE COMPARISION
|NAME|P100|M40|K40|
|:--:|:---:|:----:|:----:|
|Architecture|Pascal|Maxwell|Kepler|
|Double Precision(FP64)|5.3 Tflop/s|0.2 Tflops/s|1.4 Tflops/s|
|Single Precision(FP32)|10.6 Tflop/s|7 Tflop/s|4.3 Tflop/s|
|Half Precision(FP16)|21.1 Tflop/s|N/A|N/A|
|Memory Bandwidth|720 GB/s|288 GB/s|288 GB/s|
|Memory Size|16 GB|12 GB/24 GB|12 GB|

# VOLTA V100
* 84 streaming Multiprocessors (SM's)
* 5,376 GPU Cores
* 672 Tensor Cores(i.e. Google TPU)
  * Mixed FP16/FP32 precision
* More shared Memory
* New L0 Instruction Cache
* Faster L1 Data Cache
* V100 vs. P100 Performance
  * 12x TFLOPS@Peak Training
  * 6x inference Throughput

# V100 AND CUDA 9
* Independent Thread Scheduling
  * Similar to CPU fine-grained thread synchronization semantics
  * Allow GPU to yield execution of any thread
* Still Optimized for SMIT (same Instruction Multiple Thread)
  * SMIT units automatically scheduled together
* Explicit synchronization

# CUDA STREAMS
* Asynchronous I/O Trnasfer
* Overlap Compute and I/O
* Keep GPUs Saturated
* Fundmaental to Queue Framework in TensorFlow


