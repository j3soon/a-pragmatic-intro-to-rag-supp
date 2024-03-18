# A Pragmatic Intro to RAG, Supplementary Materials

This repo contains supplementary materials for the talk "A Pragmatic Introduction to Retrieval-Augmented-Generation (RAG)".

1. Hands-on code for RAG [[here](https://github.com/Squirtle007/Retrieval-Augmented_Generation)]
2. Post-talk Survey [[here](https://forms.gle/7dhAsdkaQJGabN4S6)]
3. (Optional) Register GTC 2024 online for free [[here](https://www.nvidia.com/gtc/?ncid=GTC-NVOLV917)]
   - [Transforming AI [S63046]](https://www.nvidia.com/gtc/session-catalog/?search=S63046&tab.allsessions=1700692987788001F1cG#/session/1702594702652001JJhD)
   - [Gaming Conference Sessions](https://www.nvidia.com/gtc/sessions/gaming/)
4. Going Further
   - [NVIDIA/GenerativeAIExamples](https://github.com/NVIDIA/GenerativeAIExamples)
     - [RAG in 5 minutes example](https://github.com/NVIDIA/GenerativeAIExamples/tree/main/examples)
   - [Building RAG Agents with LLMs](https://courses.nvidia.com/courses/course-v1:DLI+S-FX-15+V1/)

## Abstract of the Talk

Pre-trained large language models (LLMs) have demonstrated great potential in language generation. However, certain challenges persist, such as providing the sources that influence their decisions, staying current with the latest knowledge, handling knowledge-intensive tasks, and mitigating "hallucinations". To tackle these challenges, Retrieval-Augmented-Generation (RAG) has emerged as a promising paradigm, where a parametric LLM specialized in language generation collaborates with traditional non-parametric vector databases.

RAG involves two key processes: (1) Document ingestion from external repositories, databases, or APIs beyond the foundational model's knowledge. (2) Retrieval of relevant document data and response generation during inference. In the first process, documents from the knowledge database are encoded by an embedding model, converting their content into vectors. These vector embeddings are then stored in a dedicated vector database. In the second process, the user's query is transformed into vectors using the same embedding model utilized in the previous step. The vector database performs a similarity search to identify vectors closely aligning with the user's intent, providing them to the Language Model (LLM) for context enhancement.

After introducing the core concepts and components of RAG in the main presentation, attendees will be guided through a hands-on session featuring a simplified RAG example. The only prerequisite for attendees is a laptop with an internet connection. During this session, participants will execute code on Google Colab, leveraging free API endpoints for accessing LLMs. This exercise aims to offer participants practical experience in building a basic RAG system using popular open-source libraries.

Lastly, a curated list of resources is provided for individuals interested in delving deeper into RAG. Those intrigued by this topic can explore these materials to gain further insights into the latest research trends on RAG and follow the documentations to develop their own RAG applications.
