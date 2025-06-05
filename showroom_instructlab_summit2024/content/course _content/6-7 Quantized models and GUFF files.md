# Quantized Models and GUFF Files

# :bulb:Quantized Model 

[More information at huggingface.com](https://huggingface.co/docs/optimum/en/concept_guides/quantization)


Quantization is a technique to reduce the computational and memory costs of running inference by representing the weights and activations with low-precision data types like 8-bit integer (int8) instead of the usual 32-bit floating point (float32).

Reducing the number of bits means the resulting model requires less memory storage, consumes less energy (in theory), and operations like matrix multiplication can be performed much faster with integer arithmetic. It also allows to run models on embedded devices, which sometimes only support integer data types.





# :bulb:GGUF files (GPT-Generated Unified Format)


Then Hugging Face Hub (where you can access many open source models), supports many file formats, but has built-in features for [GGUF format](https://github.com/ggerganov/ggml/blob/master/docs/gguf.md), a binary format that is optimized for quick loading and saving of models, making it highly efficient for inference purposes. GGUF is designed for use with GGML and other executors. GGUF was developed by [@ggerganov](https://huggingface.co/ggerganov) who is also the developer of [llama.cpp](https://github.com/ggerganov/llama.cpp), a popular C/C++ LLM inference framework. Models initially developed in frameworks like PyTorch can be converted to GGUF format for use with those engines.

Further Reading [More information at huggingface.com](https://huggingface.co/docs/hub/en/gguf)


## What are GUFF files?

GPT-Generated Unified Format (GGUF) is a file format that streamlines the use and deployment of large language models (LLMs). GGUF is specially designed to store inference models and perform well on consumer-grade computer hardware.

Further reading: [GGUF versus GGML](https://www.ibm.com/think/topics/gguf-versus-ggml) by [Tim Mucci](https://www.ibm.com/think/author/tim-mucci)