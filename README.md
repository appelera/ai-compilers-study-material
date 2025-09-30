## AI compilers studying materials 

### Description
This repository is intended to help someone who wants to start working on the fields of AI compilers and systems.

By "AI compilers", I've meant a SW stack which translates and optimizes DNN models into assembly at accelerators, such as GPUs or NPUs.

I've curated the most useful resources I've found so far.

### Prerequisites
- Basic understanding of DNN and Transformer architectures.
- Some experience on parallel programming and GPUs (e.g., implementing matmul on CUDA).

### High-level ideas
-  https://huyenchip.com/2021/09/07/a-friendly-introduction-to-machine-learning-compilers-and-optimizers.html
- https://www.modular.com/blog/democratizing-ai-compute-part-6-what-about-ai-compilers
  - Strongly recommend to read the full series
- https://docs.google.com/presentation/d/1RZdV3Z-Q1NEbpU1-qk9C97yE1QvwNLJ9Gc7JLaFLZCw/edit?slide=id.p#slide=id.p

### Papers
- [List of papers](https://github.com/merrymercy/awesome-tensor-compilers)
- There is [a survey paper](https://arxiv.org/abs/2002.03794), but keep in mind that it is a bit outdated (2020).
- I'd recommend reading recent ML/DNN/AI compiler papers on ASPLOS/MLSys/PLDI/ISCA, such as:
  - https://arxiv.org/pdf/2311.02103
  - https://arxiv.org/pdf/2504.07004
  - https://arxiv.org/pdf/2411.07211
- FlashAttention series are also recommended to understand the gist of kernel optimization for LLMs.
  - https://arxiv.org/pdf/2205.14135
  - https://arxiv.org/pdf/2307.08691
  - https://arxiv.org/pdf/2407.08608
  - https://arxiv.org/pdf/2311.01282

### Open-source projects
- [TVM](https://github.com/apache/tvm) and [XLA](https://github.com/openxla/xla) are the OG open-source standards, but their popularity seems like going down these days.
- At the state of 2025, PyTorch 2 compilers[[paper](https://dl.acm.org/doi/abs/10.1145/3620665.3640366)][[repo](https://github.com/pytorch/pytorch/tree/main/torch/_inductor)] with Triton[[paper](https://www.eecs.harvard.edu/~htk/publication/2019-mapl-tillet-kung-cox.pdf)][[repo](https://github.com/triton-lang/triton)] are a good choice.
- For more lower-level GPU optimizations (lower than Triton yet higher than CUDA), refer to [CUTLASS](https://docs.nvidia.com/cutlass/index.html).

### Hands-on tutorials
- TVM
  - https://mlc.ai/
  - https://tvm.d2l.ai/
- Triton
  - https://github.com/srush/Triton-Puzzles
  - https://triton-lang.org/main/getting-started/tutorials/index.html
- PyTorch 2 compilers
  - https://github.com/meta-pytorch/workshops/tree/master/ASPLOS_2024
  - https://docs.google.com/document/d/1zY9Nlmh5jT39Q92aDYf3dHOAXh2xCMdeS6pnbX0Dqpw/edit?tab=t.0#heading=h.8exgp9nti6e2
 
### Other useful materials
- [GPU MODE Youtube channel](https://www.youtube.com/@GPUMODE)
- [AI compilers study](https://carpedm30.notion.site/AI-Compiler-Study-aaf4cff2c8734e50ad95ac6230dbd80b)
- [Matrix Multiplication on Blackwell](https://www.modular.com/categories/engineering)
- [How to Scale Your Model: A Systems View of LLMs on TPUs](https://jax-ml.github.io/scaling-book/)
- [Domain-specific architectures for AI inference](https://fleetwood.dev/posts/domain-specific-architectures)
