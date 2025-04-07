# running_llm_on_cpu_quantization
This project demonstrates a proof of concept for quantization by running the LLaMA model on a standard CPU-based machine. LLaMA (Large Language Model Meta AI), developed by Meta, is a state-of-the-art large language model designed for natural language processing tasks. Even the smallest version, LLaMA-7B, contains 7 billion parameters, and larger versions like LLaMA-13B, 30B, and 65B are significantly more resource-intensive.

Due to its size, running LLaMA on machines with limited resources (like CPUs) is challenging. This proof of concept explores how quantization, a core computer science concept, can be used to reduce the memory footprint of the model by converting high-precision floating-point weights (float32) into lower-precision integer types (int8), significantly shrinking the model size.

For example:

1. A float32 model with 1 million weights would typically require ~4MB of RAM.

2. After quantization to int8, the same model would require only ~1MB — a 75% reduction in memory usage.

Of course, this comes with trade-offs. Quantization sacrifices some accuracy, as it reduces the numerical precision of the model. However, it can lead to faster inference times, especially on resource-constrained systems.

If speed and memory efficiency are the priority — such as when deploying models to mobile or edge devices — quantization is an excellent approach, even if it comes at the cost of some accuracy.

This project aims to highlight the practical application of quantization in making large-scale models like LLaMA more accessible and efficient for low-resource environments.
