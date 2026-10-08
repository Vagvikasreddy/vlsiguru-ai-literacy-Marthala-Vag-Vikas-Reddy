# Mission 7 - What Actually Runs AI?

## Objective

The objective of this mission is to understand the hardware that makes Artificial Intelligence possible. AI models do not run by themselves. They require computing hardware such as CPUs, GPUs, and AI accelerators to process large amounts of data efficiently.

## Answer

A **CPU (Central Processing Unit)** is the main processor of a computer. It is designed to perform many different types of tasks and is good at handling general-purpose operations. Every computer has a CPU, and it manages the operating system, applications, and other everyday tasks. Although a CPU can run AI models, it is not the fastest option for very large AI workloads.

A **GPU (Graphics Processing Unit)** was originally designed for graphics processing, but it is also very good at AI because it can perform thousands of calculations at the same time. This is called **parallel computation**. Instead of processing one calculation after another like a CPU, a GPU can process many calculations simultaneously. This makes GPUs much faster for training Deep Learning models.

An **NPU (Neural Processing Unit)** or **AI Accelerator** is specialized hardware designed specifically for AI workloads. It is optimized to perform AI operations more efficiently while using less power. Modern smartphones and laptops include NPUs to run AI features such as face recognition, image enhancement, and voice assistants.

AI depends heavily on compute power and memory because modern AI models process very large datasets and perform billions of mathematical calculations during training. Training a model requires much more computation than inference because the model is continuously learning from data and updating its internal parameters. During **inference**, the trained model only generates predictions or responses using the knowledge it has already learned, so it requires less computation.

## AI Hardware Diagram

```text
AI Application
       │
       ▼
AI Model
       │
       ▼
Software / Framework
       │
       ▼
CPU / GPU / NPU
       │
       ▼
Memory
```

## Real AI Workload

**AI Workload:** Training ChatGPT or another Large Language Model

**Best Hardware:** GPU

**Reason:** Training a Large Language Model requires processing huge amounts of data and performing billions of mathematical calculations in parallel. GPUs are designed for this type of workload and can complete the training much faster than CPUs.

## Conclusion

This mission helped me understand that AI models need powerful hardware to process data efficiently. CPUs are useful for general computing, GPUs are better for training AI models because of parallel computation, and NPUs are specialized processors designed to run AI tasks efficiently on modern devices.
