\# Experiment 6 – CUDA Programming



\## Aim

To implement and analyze matrix transpose and matrix multiplication using CUDA.



\## GPU Details

\- GPU: NVIDIA RTX 4500 Ada Generation

\- Compute Capability: 8.9

\- CUDA Toolkit: 13.4



\## Programs Implemented

1\. Naive Matrix Transpose

2\. Coalesced Matrix Transpose using Shared Memory

3\. Naive Matrix Multiplication



\## Performance Results



| Operation | Execution Time |

|---|---:|

| Uncoalesced Transpose | 0.730 ms |

| Coalesced Transpose | 0.368 ms |

| Naive Matrix Multiplication | 0.894 ms |



Matrix Multiplication Performance: 2401.8 GFLOPS



Coalesced Transpose Speedup: 1.98x



\## Compilation



nvcc -O2 -arch=sm\_89 -o exp6.exe exp6.cu



\## Execution



exp6.exe



\## Conclusion

The experiment demonstrates CUDA parallel programming, matrix operations, and the performance benefits of coalesced memory access.

