## Getting started

**GPU in ML:** Deep learning requires fast matrix computations and FLOPs (Floating Point Operations) per second and parallel computations for rendering, which GPUs are highly optimised for.

**Nvidia is better:** Native pytorch CUDA support. More suitable for cuDNN.

Cell [1]: `import torch`  
`t_cpu = torch.rand(500,500,500)`  
`%timeit t_cpu @ t_cpu`

Cell [2]: `t_gpu = torch.rand(500,500,500).cuda()`  
`%timeit t_gpu @ t_gpu`
