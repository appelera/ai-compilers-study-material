## AI compilers studying materials 

### High-level ideas
- https://huyenchip.com/2021/09/07/a-friendly-introduction-to-machine-learning-compilers-and-optimizers.html
- https://www.modular.com/blog/democratizing-ai-compute-part-6-what-about-ai-compilers
  - Strongly recommend to read the full series
- https://docs.google.com/presentation/d/1RZdV3Z-Q1NEbpU1-qk9C97yE1QvwNLJ9Gc7JLaFLZCw/edit?slide=id.p#slide=id.p

### Papers
- List of papers
  - https://github.com/merrymercy/awesome-tensor-compilers?tab=readme-ov-file#compiler-and-ir-design
  - https://carpedm30.notion.site/AI-Compiler-Study-aaf4cff2c8734e50ad95ac6230dbd80b
- Although there is [a survey paper](https://arxiv.org/abs/2002.03794), it is a bit outdated (2020).
- So I'd rather recommend reading recent ML/DL/AI compiler papers on ASPLOS/MLSys/PLDI, such as:
  - https://arxiv.org/abs/1802.04799
  - https://arxiv.org/pdf/2411.07211
  - https://arxiv.org/pdf/2311.02103
  - https://arxiv.org/pdf/2504.07004
- FlashAttention series are also recommended to understand the gist of kernel optimization for Transformers / LLMs.
  - https://arxiv.org/pdf/2205.14135
  - https://arxiv.org/pdf/2307.08691
  - https://arxiv.org/pdf/2407.08608
  - https://arxiv.org/pdf/2311.01282

### Open-source projects
- TVM and XLA are the OG open-source standards, but their popularity is going down these days.
- At the state of 2025, PyTorch 2 compilers + Triton is worth looking at
  - paper: https://dl.acm.org/doi/abs/10.1145/3620665.3640366, https://www.eecs.harvard.edu/~htk/publication/2019-mapl-tillet-kung-cox.pdf
  - repo: https://github.com/pytorch/pytorch/tree/main/torch/_inductor, https://github.com/triton-lang/triton
- Or [CUTLASS and CuTe](https://docs.nvidia.com/cutlass/index.html)

### Hands-on tutorials
- TVM
  - https://mlc.ai/
  - https://tvm.d2l.ai/
- Triton
  - https://triton-lang.org/main/getting-started/tutorials/index.html
  - https://github.com/srush/Triton-Puzzles
- TorchInductor
  - https://docs.google.com/document/d/1zY9Nlmh5jT39Q92aDYf3dHOAXh2xCMdeS6pnbX0Dqpw/edit?tab=t.0#heading=h.8exgp9nti6e2
