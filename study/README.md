# Study Notes

## Von Neumann Bottleneck

Processor and memory are physically separate, so data movement can limit system performance even when compute capability grows.

## GPU

GPUs provide many parallel execution units and are well suited to large data-parallel workloads such as AI training and inference.

## HBM

High Bandwidth Memory stacks DRAM dies vertically and uses short high-density interconnects to increase bandwidth near compute devices.

From a process perspective, HBM depends heavily on TSV, thinning, bonding, thermal design, and yield.

## Quantum Computing

Quantum computing uses quantum states such as superposition and entanglement.

It is not simply a faster CPU. Its advantage is problem-specific and depends on algorithms, hardware fidelity, control, and error correction.

## Quantum–Classical Hybrid

A hybrid system uses classical CPU/GPU/HPC resources for orchestration and conventional workloads, while assigning selected tasks to QPUs.

## Neuromorphic Computing

Neuromorphic systems imitate aspects of biological information processing.

Common research themes include event-driven operation, in-memory computing, synaptic devices, and memristive arrays.

## Heterogeneous Integration

Different compute and memory technologies can be combined at system/package level to match each workload with the most suitable hardware.

This is a recurring theme connecting HBM, AI accelerators, and quantum-centric supercomputing.
