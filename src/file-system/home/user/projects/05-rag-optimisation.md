



## *Optimizing Retrieval-Augmented Generation (RAG) Pipelines*

### • Python, LangChain, Milvus, Sentence Transformers  
### • FLAN-T5, Prompt Engineering, Evaluation Metrics  

Designed, implemented, and evaluated a Retrieval-Augmented Generation (RAG) system through multiple experimental phases to benchmark embedding models, prompt strategies, and advanced retrieval techniques.  

The baseline pipeline compared two embedding models — *all-MiniLM-L6-v2 (384d)* and *all-mpnet-base-v2 (768d)* — across Instruction, Persona, and Chain-of-Thought prompts. The 768d model achieved an **F1 score of 81%**, outperforming the smaller model (77%). The **Persona prompt** yielded the best performance, while Chain-of-Thought consistently degraded output quality.  

An advanced RAG version introduced **query rewriting** and **cross-encoder reranking** for semantic precision. However, experiments revealed that increased complexity reduced performance (average F1 dropped from 73.6% to 69.6%), emphasizing the importance of **strategic simplicity and prompt optimization** in RAG systems.  

**System Highlights:**
- Integrated **Milvus Lite** for vector search with L2 similarity.  
- Used **google/flan-t5-base** for generation and query rewriting.  
- Evaluated across varying top-k retrievals, finding **k=3** optimal.  
- Proposed **production deployment** strategies including distributed vector DBs and GPU inference scaling.  

This project deepened my expertise in **end-to-end RAG architecture**, **prompt strategy evaluation**, and **model efficiency trade-offs** for real-world deployment.
