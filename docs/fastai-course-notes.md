# fast.ai coursenotes

*Learnings from the fast.ai course*

## Time stopped: ~60 min / 1,40 hrs (Already finished but need to tick off the below to finish)

## Getting started

**GPU in ML:** Deep learning requires fast matrix computations and FLOPs (Floating Point Operations) per second and parallel computations for rendering, which GPUs are highly optimised for.

**Nvidia is better:** Native pytorch CUDA support. More suitable for cuDNN.

Cell [1]: `import torch`  
`t_cpu = torch.rand(500,500,500)`  
`%timeit t_cpu @ t_cpu`

Cell [2]: `t_gpu = torch.rand(500,500,500).cuda()`  
`%timeit t_gpu @ t_gpu`

## Setup (Kaggle + GCP)

* ⭕ Going to use GCP - need to install cloud or read manual (check email) to setup VM instance

* ⭕ Readup on regex

* ⭕ FInish notebook 

---

## Common misconceptions

**Black box:** Interprable ML, visualise gradients + activations

**Needs too much data:** Transfer learning, share pre-trained nets

**Needs GPUs:** Only for some research project

---

## Lesson 1

**Dataset:** Going to use either *academic* or *kaggle* datasets as they give us a strong baseline for performance and what is currently state of the art (i.e. via papers, kaggle compteition results). We will use square datasets, part 2 rectangular images.

**Context:** It was hard in the 80s for a dogs vs cats problem but now it is too easy. We are going to perform the below - 

**Task:** Fine-grain classification (term for distinguishing betwen categories)

**On GPUs:** GPU perfrms fast by giving same set of instructions. So data has to be standerdised (i.e. in dimension)

**Model:** Resnet34 (34 layers) is good enough, ranks consistently as top 5 performer (2016)



**L1 jupyter notebook reference from the github account**

vision.data.ipyng
