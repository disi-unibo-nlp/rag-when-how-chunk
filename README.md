# **Reconstructing Context: Evaluating Advanced Chunking Strategies for Retrieval-Augmented Generation**

## **Overview**
This repository contains the implementation and analysis of two retrieval strategies for maintaining context in document retrieval: **Late Chunking** and **Contextual Retrieval**. While both approaches effectively mitigate the **context-dilemma**, neither provides a definitive solution, as each comes with trade-offs in efficiency and performance.

- **Late Chunking**: More computationally efficient, leveraging embedding models' natural capabilities for chunk-wise representation.
- **Contextual Retrieval**: Provides better context augmentation and re-ranking through LLMs but incurs higher computational costs.

## **Methodology**
We evaluated both approaches using two datasets: **NFCorpus** and **MSMARCO**, chosen because no other publicly available datasets allowed for proper benchmarking of the retrieval component. The evaluation focused on:
- **Computational Efficiency**: Measuring the resource consumption of each approach.
- **Retrieval Quality**: Assessing the ability to preserve document context.
- **Impact of Model Choice**: Analyzing the effect of different LLM sizes and efficiency.

## **Limitations**
- Our results are constrained to NFCorpus and MSMARCO, which may **limit the generalizability** of our findings.
- The **trade-offs between efficiency and semantic coherence** are well-established in prior research, making the conclusions somewhat expected.
- Future work should **explore additional datasets** to derive broader insights and validate these findings across different retrieval tasks.

## **Future Work**
To enhance the study, potential improvements include:
- Expanding experiments to a wider range of **datasets**.
- Investigating alternative **retrieval strategies** beyond late chunking and contextual retrieval.
- Exploring optimization techniques for balancing **efficiency vs. retrieval quality** in real-world applications.

## **Installation & Usage**
To replicate the experiments, follow these steps:

### **Requirements**
- Python 3.x
- PyTorch
- Transformers (Hugging Face)
- Faiss (for efficient similarity search)

### **Installation**
```bash
git clone https://github.com/your-repo/context-retrieval.git
cd context-retrieval
pip install -r requirements.txt
```

# rag-late-contextual
[AI Project Work, KEIR] When and How Chunk in Modern RAG Applications

Python notebooks, compiled on Google Colab using local resources with RTX-4090
