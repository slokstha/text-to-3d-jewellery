# Setup Notes

## Environment

- Device: MacBook Air
- OS: macOS
- Python Virtual Environment configured successfully

---

## DreamFusion Installation Attempt

Stable DreamFusion dependencies were partially installed successfully.

However, CUDA-dependent packages such as:

- nvdiffrast
- tinycudann
- CUDA rendering extensions

cannot be compiled locally on macOS because the project is primarily designed for NVIDIA CUDA environments.

---

## Engineering Observation

This highlighted an important deployment consideration in generative AI systems:

Many state-of-the-art 3D generative pipelines depend heavily on CUDA-based acceleration and are optimised for Linux + NVIDIA GPU environments.

---

## Planned Next Steps

- Continue local experimentation where possible
- Use cloud GPU environments for full pipeline execution
- Explore lightweight NeRF-compatible workflows on macOS
- Document rendering outputs and inference observations