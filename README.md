# Hate Speech Detection Using Multi LLM Architecture

Final Project for CS6501-011 Natural Language Processing at University Of Virginia

### Contributors

Sravanth Chowdary Potluri

Darsh Naresh Jain

Asjad Nirban

### Abstract

This project presents a two-tiered multi-LLM architecture for detecting and categorizing hate speech in social media text, addressing the computational inefficiencies of single large models. The approach utilizes a smaller LLaMA 1B model for initial binary classification to efficiently filter non-hateful content, while the larger LLaMA 3B model is selectively invoked for fine-grained categorization of detected hateful content. Experiments on a benchmark dataset demonstrate significant computational benefits, achieving an 18% improvement in processing time and a 54% reduction in memory usage compared to using the larger model alone. These improvements are driven by the selective use of the resource-intensive model, which reduces overhead without major performance sacrifices. However, the combined accuracy of the two-tier system depends on the reliability of the smaller model; misclassifications at the first stage may prevent the second model from being triggered, leading to potential gaps in performance. Future work includes enhancing the smaller model’s calibration, exploring LoRA/QLoRA for efficient fine-tuning, and implementing adaptive thresholds for real-world adaptability. This architecture provides a scalable and resource-efficient solution for hate speech detection, offering broader applicability to hierarchical classification tasks across various NLP domains.
