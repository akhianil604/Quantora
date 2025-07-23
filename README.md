# Elemental Adaptation of LR-QAT for LLMs on NLP Tasks
## Authors
1. **Akhilesh Anil***
2. **Chinmay Shivanand Muragod***
3. **Vinod G R***
4. **Sujatha R Upadhyaya*** <br/>
*Centre of Data Sciences & Applied Machine Learning, PES University, Bangalore, India

## Our Implementation 
1. Render Pre-trained frozen weight matrix using [LR-QAT](https://arxiv.org/abs/2406.06385)
2. Training of LoRA adapters & Quantisation parameters over the quantisation grid.
3. Fusion of LoRA adapters with the frozen weight matrix to generate a full-precision merged model.
4. Progressive quantisation of merged model to BF16, INT8 & NF4 precisions.

## Experimental Setup
*Platform for Training & Evaluation*: Google Colab's Nvidia 15 GB T4 GPU.<br/>
*Datasets*: SST-2 & QNLI tasks from GLUE benchmark dataset.<br/>
*Models*: GPT-2 Medium (355 M parameters) & BERT-Base-Uncased (110 M parameters)<br/>
