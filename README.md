## AI compilers study materials 

### Description
This repository is designed as a focused resource for individuals beginning work in the field of AI compilers and systems.

​By AI compilers, I specifically refer to the software stack responsible for translating and optimizing DNN models into efficient assembly code for various accelerators, including GPUs and NPUs.

​I have curated the most valuable resources I've encountered to date—including two original materials I developed—to provide a solid starting point.

### Prerequisites
- Basic understanding of DNN and Transformer architectures.
- Some experience on parallel programming and GPUs (e.g., implementing matmul on CUDA).

### High-level ideas
- [A friendly introduction to machine learning compilers and optimizers](https://huyenchip.com/2021/09/07/a-friendly-introduction-to-machine-learning-compilers-and-optimizers.html)
- [Democratizing AI compute: Part 6](https://www.modular.com/blog/democratizing-ai-compute-part-6-what-about-ai-compilers)
  - Strongly recommend to read the full series
- [Introduction to AI compilers](https://docs.google.com/presentation/d/1RZdV3Z-Q1NEbpU1-qk9C97yE1QvwNLJ9Gc7JLaFLZCw/edit?slide=id.p#slide=id.p)

### Papers
- [List of papers](https://github.com/merrymercy/awesome-tensor-compilers)
- There is [a survey paper](https://arxiv.org/abs/2002.03794), but keep in mind that it is a bit outdated (2020).
- I'd recommend skimming through recent ML/DNN/AI compiler papers on ASPLOS/MLSys/PLDI/ISCA, such as [Relax](https://arxiv.org/pdf/2311.02103), [Cypress](https://arxiv.org/pdf/2504.07004), [Exo2](https://arxiv.org/pdf/2411.07211).
- FlashAttention series are also recommended to understand the gist of kernel optimization for LLMs[[1](https://arxiv.org/pdf/2205.14135)][[2](https://arxiv.org/pdf/2307.08691)][[3](https://arxiv.org/pdf/2407.08608)][[decoding](https://arxiv.org/pdf/2311.01282)].

### Open-source projects
- [TVM](https://github.com/apache/tvm) and [XLA](https://github.com/openxla/xla) are the OG open-source standards, but their popularity seems like going down these days.
- At the state of 2025, PyTorch 2 compilers[[paper](https://dl.acm.org/doi/pdf/10.1145/3620665.3640366)][[repo](https://github.com/pytorch/pytorch/tree/main/torch/_inductor)] with Triton[[paper](https://www.eecs.harvard.edu/~htk/publication/2019-mapl-tillet-kung-cox.pdf)][[repo](https://github.com/triton-lang/triton)] can be a good choice.
- For more lower-level GPU optimizations (lower than Triton yet higher than CUDA), refer to [CUTLASS](https://docs.nvidia.com/cutlass/index.html).
- Note on Triton:
  - For recent Hopper/Blackwell GPUs, Triton struggles to achieve optimal performance due to the increased complexity of GPU.
  - To mitigate this, [Gluon](https://github.com/triton-lang/triton/blob/main/python/tutorials/gluon/01-intro.py) is being developed within the Triton ecosystem, which exposes more lower-level controls akin to CUTLASS.

### Hands-on tutorials
- TVM
  - https://mlc.ai/
  - https://tvm.d2l.ai/
- Triton
  - https://github.com/srush/Triton-Puzzles
  - https://triton-lang.org/main/getting-started/tutorials/index.html
- PyTorch 2 compilers
  - https://github.com/meta-pytorch/workshops/tree/master/ASPLOS_2024
  - https://docs.google.com/document/d/1zY9Nlmh5jT39Q92aDYf3dHOAXh2xCMdeS6pnbX0Dqpw/edit?usp=drivesdk
 
### Other useful materials
- [GPU MODE Youtube channel](https://www.youtube.com/@GPUMODE)
- [AI compilers study](https://carpedm30.notion.site/AI-Compiler-Study-aaf4cff2c8734e50ad95ac6230dbd80b)
- [Matrix Multiplication on Blackwell](https://www.modular.com/blog/matrix-multiplication-on-nvidias-blackwell-part-1-introduction)
- [How to Scale Your Model: A Systems View of LLMs on TPUs](https://jax-ml.github.io/scaling-book/)
- [Domain-specific architectures for AI inference](https://fleetwood.dev/posts/domain-specific-architectures)
