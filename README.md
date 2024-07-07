# SEC RAG Agent: Regulatory Assistance with Transformers

![image](https://github.com/Aftabbs/SEC-RAG-Agent-Regulatory-Assistance-with-Transformers/assets/112916888/6467cd39-3111-449e-92e8-fcb3f0ba3d2d)

## Project Overview

The SEC RAG Agent (Regulatory Assistance with Transformers) is an AI-powered agent designed to assist with regulatory compliance using advanced NLP techniques and transformer-based models. It leverages Hugging Face and SEC API keys to retrieve, process, and analyze SEC filings such as 10-K and 10-Q reports. The agent utilizes sentence similarity transformers and fine-tuned models to interpret user queries, retrieve relevant information from SEC filings, and provide comprehensive answers.

## Industrial Use-Case

In industries governed by regulatory bodies like the U.S. Securities and Exchange Commission (SEC), compliance with filing regulations is crucial. The SEC RAG Agent automates and enhances the process of extracting critical information from SEC filings, including financial performance summaries, risk factors, and management discussions. This project caters to financial institutions, legal firms, and regulatory compliance departments seeking efficient, accurate, and scalable solutions for handling SEC filings.

## Key Features

### Libraries Used
- `unsloth`
- `xformers`
- `trl`
- `peft`
- `accelerate`
- `bitsandbytes`
- `sec_api`
- `langchain`
- `sentence-transformers`
- `faiss-gpu`

### Functionality

### Part 1: Fine-Tuning LLaMa 3 with Unsloth

The project fine-tunes the LLaMa 3 language model using Unsloth for parameter-efficient fine-tuning, enhancing its ability to understand and generate text relevant to SEC filings.

### Part 2: Setting Up SEC 10-K Data Pipeline & Retrieval Functionality

#### Function for 10-K Retrieval
- Utilizes the SEC API to retrieve specific sections (1A and 7) from SEC filings.
- Focuses on extracting critical information such as risk factors and management discussions.

#### Setting Up Embeddings Locally
- Embeds text chunks from SEC filings using Hugging Face embeddings.
- Defines and processes a vector database for efficient storage and retrieval of embeddings.

#### Retrieval Process
- Converts user queries into embeddings and performs similarity searches against the vector database.
- Retrieves relevant text chunks or documents based on similarity scores (cosine similarity or Euclidean distance).
- Assembles retrieved text chunks to provide coherent answers or context to user queries.

## Unique Aspects

### Hugging Face Integration
The project integrates with Hugging Face's transformer models and embeddings, utilizing state-of-the-art NLP capabilities for regulatory compliance tasks.

### Automation of Compliance Tasks
By automating the extraction and analysis of SEC filings, the SEC RAG Agent reduces manual effort, improves accuracy, and ensures timely compliance with regulatory requirements.

### Scalability and Efficiency
The use of transformer-based models and efficient retrieval techniques (like FAISS for vector storage) ensures scalability to handle large volumes of SEC filings and queries.

## Future Enhancements

Future enhancements may include:
- Integration of additional SEC filing sections for broader coverage.
- Enhancement of embedding models and similarity algorithms for improved accuracy.
- Deployment optimizations for real-time query processing and scalability.

## Conclusion

The SEC RAG Agent exemplifies the application of advanced NLP and transformer technologies in automating regulatory compliance tasks. It offers a robust solution for industries needing efficient handling of SEC filings and regulatory data.


*This project showcases the potential of AI in enhancing regulatory compliance processes, specifically tailored for industries governed by SEC regulations.*
