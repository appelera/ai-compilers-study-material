## AI compilers studying materials 

### High-level ideas
- https://huyenchip.com/2021/09/07/a-friendly-introduction-to-machine-learning-compilers-and-optimizers.html
- https://www.modular.com/blog/democratizing-ai-compute-part-6-what-about-ai-compilers

### Hands-on tutorials
- https://mlc.ai/
- (TODO) add a link to lecture
- https://triton-lang.org/main/getting-started/tutorials/index.html

### Papers
- List of papers: https://github.com/merrymercy/awesome-tensor-compilers?tab=readme-ov-file#compiler-and-ir-design
- Although there is [one survey paper](https://arxiv.org/abs/2002.03794), it is a bit outdated (2020) so I'd rather recommend reading recent ML/DL/AI compiler papers on ASPLOS, MLSys, OSDI, etc.
- Some recommended papers
  - https://arxiv.org/abs/1802.04799
  - https://arxiv.org/pdf/2411.07211
  - https://dl.acm.org/doi/10.1145/3676641.3716249

### Open-source projects
- TVM and XLA are the OG open-source standards, but their popularity is going down these days
- At the state of 2025, I think PyTorch 2 compiler (TorchDynamo + TorchInductor) + Triton is worth looking at
  - paper: https://dl.acm.org/doi/abs/10.1145/3620665.3640366, https://www.eecs.harvard.edu/~htk/publication/2019-mapl-tillet-kung-cox.pdf
  - repo: https://github.com/pytorch/pytorch/tree/main/torch/_inductor, https://github.com/triton-lang/triton
  - TorchInductor lacks documentation, so me and Gieun's [guide](https://docs.google.com/document/d/1zY9Nlmh5jT39Q92aDYf3dHOAXh2xCMdeS6pnbX0Dqpw/edit?tab=t.0#heading=h.8exgp9nti6e2) might be helpful
- Or [CUTLASS and CuTe](https://docs.nvidia.com/cutlass/index.html)
