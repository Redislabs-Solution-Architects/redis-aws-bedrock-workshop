# Redis AWS Bedrock Workshop
This hands-on workshop, aims at developers and solution builders, introduces how to leverage Redis, Redis's Vector Semantic Search, Vector Database and AWS Bedrock's base modules.

<div align="center">
    <div style="display: inline-block; text-align: center; margin-bottom: 10px;">
        <span style="font-size: 36px;"><b>Redis Vector Search: Financial Examples</b></span>
        <br />
    </div>
    <br />
</div>

<div align="center">

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
![Language](https://img.shields.io/github/languages/top/redis-developer/financial-vss)
![GitHub last commit](https://img.shields.io/github/last-commit/redis-developer/financial-vss)

</div>

Within this lab, you'll explore some of the most common usage patterns we are seeing with our customers for Generative AI. We will show techniques for generating text and images, creating value for organizations by improving productivity. This is achieved by leveraging architecting Retrieval Augumented Generation framework to help in composing emails, summarizing text, answering questions, building chatbots, and creating images. While the focus of this workshop is for you to gain hands-on experience implementing these patterns via Redis and AWS Bedrock APIs. You will also have an option of exploring integration with open-source packages like [LangChain](https://python.langchain.com/docs/integrations/vectorstores/redis).

Labs include:
- **01 - Text Generation** \[Estimated time to complete - 45 mins\]
    - Text generation with Bedrock
    - Text summarization with Titan and Claude
    - QnA with Titan
    - Entity extraction
- **02 - Knowledge bases and RAG** \[Estimated time to complete - 45 mins\]
    - Managed RAG retrieve and generate example
    - Langchain RAG retireve and generate example
- **03 - Model customization** \[Estimated time to complete - 30 mins\]
    - Coming soon
- **04 - Image and Multimodal** \[Estimated time to complete - 30 mins\]
    - Bedrock Titan image generator
    - Bedrock Stable Diffusion XL
    - Bedrock Titan Multimodal embeddings
- **05 - Agents** \[Estimated time to complete - 30 mins\]
    - Customer service agent
    - Insurance claims agent
- **06 - Open source examples (optional)** \[Estimated time to complete - 30 mins\]
    - Langchain Text Generation examples
    - Langchain KB RAG examples
    - Langchain Chatbot examples
    - NVIDIA NeMo Guardrails examples
    - NodeJS Bedrock examples

*A detailed set of Jupyter notebooks to teach semantic search and RAG patterns over public financial 10k documents with different Redis clients and integrations including: [redis-py](https://redis-py.readthedocs.io/en/stable/index.html), [redisvl](https://redisvl.com), and [langchain](https://python.langchain.com/docs/integrations/vectorstores/redis).*

# ⚡ Introduction to Vector Search in Redis
[Redis](https://redis.com), widely recognized for its low-latency performance, extends beyond traditional noSQL databases. It's uniquely suited for tasks like caching, session management, job queuing, and JSON storage. With enhanced Search+Query features, Redis emerges as a performant [Vector Database](https://redis.com/solutions/use-cases/vector-database) supporting Vector Search over unstructured data encoded as embeddings.

## 📚 Getting Started in Jupyter Notebook
Click on one of the three notebook options below to start your journey. It launches a Jupyter Notebook that prepares your environment by cloning the necessary repository artifacts, managing Python dependencies, and ends with an end-to-end walkthrough of vector search in Redis.

Select your desired notebook tutorial from below:

| # | Notebook | Description | Documentation |
|---|----------|-------------|---------------|
| 1 | [**redis-py-01**](https://colab.research.google.com/github/Redislabs-Solution-Architects/redis-aws-bedrock-workshop/blob/main/redis-py-01.ipynb) | Grasp VSS basics with the standard Redis Python client. | [View Docs](https://redis-py.readthedocs.io/en/stable/examples/search_vector_similarity_examples.html) |
| 2 | [**redisvl-02**](https://colab.research.google.com/github/Redislabs-Solution-Architects/redis-aws-bedrock-workshop/blob/main/redisvl-02.ipynb) | Dive deeper into RAG patterns from scratch using an AI-native Redis client library. | [View Docs](https://redisvl.com) |
| 3 | [**langchain-03**](https://colab.research.google.com/github/Redislabs-Solution-Architects/redis-aws-bedrock-workshop/blob/main/langchain-03.ipynb) | Wrap up with an integrated approach via LangChain. | [View Docs](https://python.langchain.com/docs/integrations/providers/redis) |


## 🛠️ Understanding the Client Ecosystem
Wondering why there are multiple clients? Each serves a unique purpose, providing varying abstraction levels. Your choice depends on several factors:

- **Use Cases**: Are you focusing on pure vector search, RAG, or other tasks like LLM semantic caching?
- **Redis Experience**: How comfortable is your team with Redis clients and commands?
- **Integration Points**: What are your touchpoints with LLMs and Embedding Providers?
- **Performance Demands**: How intensive are your performance requirements?
- **Configurability**: Do you prefer ease of use or fine-grained control?

Each notebook explores these considerations, guiding you through making an informed choice for your use case.

## ⚠️ Cautionary Advice
- **Not for Local Use**: This Colab-centric project isn't configured for local environments. Running it outside Colab requires a different setup.
- **Temporary Workspace**: Colab doesn't save your work indefinitely. Download your notebooks or save them to Google Drive to avoid losing progress.
- **Idle Disconnections**: Extended inactivity in Colab can disconnect the runtime, potentially resulting in work loss. Regular saving is your friend!
