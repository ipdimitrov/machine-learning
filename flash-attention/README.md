# Machine Learning Projects

This repository contains machine learning implementations focusing on Flash Attention using Triton.

## Projects

| Project | Status |
|---------|--------|
| Implementing Flash Attention in Python using Triton | ✅ **Completed** |
| Instructions for running Triton and CUDA code locally | ✅ **Completed** |
| [Blog post](https://dimitrov.substack.com/p/implementing-flash-attention) explaining Flash Attention implementation| ✅ **Completed**  |
| Shell scripts to run and benchmark Flash Attention | Not Started |
| Implementing Matrix Multiplication using Triton | Not Started |
| Implementing Layer Normalization using Triton | Not Started |

## Flash Attention Implementation

This project implements the Flash Attention algorithm using Triton. Flash Attention is an efficient attention mechanism that reduces memory usage and improves performance for transformer models.

### Instructions for running the code

#### Setup and Installation for flash-attention/triton

1. Create a new virtual environment:
   ```bash
   # For Linux/macOS
   python3 -m venv venv
   
   # For Windows
   python -m venv venv
   ```

2. Activate the virtual environment:
   ```bash
   # For Linux/macOS
   source venv/bin/activate
   
   # For Windows
   venv\Scripts\activate
   ```

3. Install the required dependencies:
   ```bash
   pip install -r flash-attention/requirements.txt
   ```

4. Run the Flash Attention implementation:
   ```bash
   # For Linux/macOS
   python3 flash-attention/triton/flash-attention.py
   
   # For Windows
   python flash-attention/triton/flash-attention.py
   ```

#### Setup and Installation for flash-attention/cuda

1. Make sure you have CUDA toolkit installed on your system. You can download it from the [NVIDIA CUDA Toolkit website](https://developer.nvidia.com/cuda-downloads).

2. Navigate to the CUDA directory:
   ```bash
   cd flash-attention/cuda
   ```

3. Build the CUDA examples:
   ```bash
   make build
   ```

Note: The CUDA examples require a NVIDIA GPU with CUDA support. Make sure your system meets the requirements before running the code.



### Resources
- [Triton documentation](https://triton-lang.org/main/index.html)
- [Reference implementation](https://github.com/hkproj/triton-flash-attention)
- [Tutorial video](https://www.youtube.com/watch?v=zy8ChVd_oTM)

### Next Steps
- Create blog post explaining the implementation details
- Add benchmarking against PyTorch's native attention
- Add shell scripts for easy execution and benchmarking
- Create instructions on how to run the CUDA code in this repository locally
- Implement additional Triton examples (Matrix Multiplication, Layer Normalization)

---
Shield: [![CC BY-NC 4.0][cc-by-nc-shield]][cc-by-nc]

This work is licensed under a
[Creative Commons Attribution-NonCommercial 4.0 International License][cc-by-nc].

[![CC BY-NC 4.0][cc-by-nc-image]][cc-by-nc]

[cc-by-nc]: https://creativecommons.org/licenses/by-nc/4.0/
[cc-by-nc-image]: https://licensebuttons.net/l/by-nc/4.0/88x31.png
[cc-by-nc-shield]: https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey.svg


