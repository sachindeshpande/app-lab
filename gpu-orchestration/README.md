# GPU Orchestration

A learning project exploring the fundamentals of GPU orchestration — how to discover, allocate, schedule, and manage GPU resources across workloads.

## Learning Goals

- Understand GPU hardware basics (cores, memory, compute capability)
- Query and monitor GPU resources programmatically
- Run workloads on specific GPUs
- Explore multi-GPU task distribution
- Learn scheduling strategies (round-robin, memory-aware, priority-based)
- Understand frameworks and tools used in production GPU orchestration

## Topics to Explore

### 1. GPU Discovery & Monitoring
- Querying available GPUs with `nvidia-smi` and `pynvml`
- Reading utilization, memory, temperature, and power stats

### 2. Basic GPU Assignment
- Assigning workloads to specific GPUs via `CUDA_VISIBLE_DEVICES`
- Running PyTorch / TensorFlow on a target device

### 3. Multi-GPU Workloads
- Data parallelism basics
- `torch.nn.DataParallel` and `DistributedDataParallel`

### 4. Orchestration Frameworks
- Overview of Kubernetes + NVIDIA device plugin
- Ray for distributed GPU workloads
- SLURM GPU scheduling basics
- Triton Inference Server for model serving

### 5. Resource Management
- GPU memory management and OOM handling
- Time-slicing and MPS (Multi-Process Service)
- Monitoring and alerting patterns

## Prerequisites

- Python 3.10+
- Access to a machine with one or more NVIDIA GPUs (or a cloud GPU instance)
- CUDA toolkit installed
- `pip install pynvml torch`

## Project Structure

```
gpu-orchestration/
├── README.md
├── 01-discovery/       # GPU querying and monitoring scripts
├── 02-assignment/      # Running workloads on specific GPUs
├── 03-multi-gpu/       # Data parallelism experiments
├── 04-orchestration/   # Framework exploration (Ray, K8s, etc.)
└── 05-management/      # Memory management and scheduling
```

## Resources

- [NVIDIA CUDA Programming Guide](https://docs.nvidia.com/cuda/cuda-c-programming-guide/)
- [PyTorch Distributed Overview](https://pytorch.org/tutorials/beginner/dist_overview.html)
- [Ray Documentation](https://docs.ray.io/)
- [Kubernetes GPU Scheduling](https://kubernetes.io/docs/tasks/manage-gpus/scheduling-gpus/)

## Status

🟡 In Progress — Setting up foundational scripts
