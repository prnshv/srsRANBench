# srsRANBench: An Open Source Benchmark for Assessing an LLMs for the srsRAN Project

## Introduction  

**srsRANBench** builds on the framework of ORAN-Bench-13K to introduce a novel benchmark specifically designed for evaluating Large Language Models (LLMs) in the context of code generation and code understanding for the **srsRAN** project. This benchmark consists of **1,502** samples, carefully curated by randomly selecting C++ files from the entire srsRAN codebase.  

The benchmark assesses LLMs' ability to generate syntactically and semantically correct code, as well as their comprehension of the srsRAN codebase. By ensuring a randomized selection process, srsRANBench provides a representative and unbiased evaluation, making it a valuable tool for both academia and industry. The dataset is designed to be computationally efficient while still capturing the complexity of real-world 5G O-RAN coding tasks.  

This work is a part of our work for foundational O-RAN LLMs called **ORANSight-2.0**, the manuscript detailing srsRANBench and ORANSight-2.0 will be available soon. Meanwhile, if you use this benchmark in your research, please cite our previous work:  

```bibtex
@misc{gajjar2024oranbench13kopensourcebenchmark,
      title={ORAN-Bench-13K: An Open Source Benchmark for Assessing LLMs in Open Radio Access Networks}, 
      author={Pranshav Gajjar and Vijay K. Shah},
      year={2024},
      eprint={2407.06245},
      archivePrefix={arXiv},
      primaryClass={cs.NI},
      url={https://arxiv.org/abs/2407.06245}, 
}
```  

## Motivation  

The **srsRAN** project is an open-source, widely used **5G O-RAN stack**, leveraged by both academia and industry for research, development, and real-world deployments. With the increasing reliance on AI-driven coding assistants, **srsRANBench** provides a critical evaluation tool for assessing how well LLMs perform in **5G O-RAN-specific coding tasks**.  

## Repository Structure  

- **Benchmark**: The MCQA benchmark consists of **1,502** high-quality questions serving as the evaluation set for LLM-generated code and understanding tasks.  
## Contribution  

We welcome contributions to expand and refine srsRANBench. If you have suggestions or would like to contribute additional tasks, please reach out to us.  

## License  

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for more details.  
