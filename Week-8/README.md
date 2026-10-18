# Healthcare Administrative AI Assistant
An integrated LLM system that classifies patient administrative requests, retrieves policy evidence, routes safe workflow actions, and produces grounded responses.

## Architecture
The project uses a modular LLM architecture to process healthcare administrative requests through the following pipeline:
User Request → Dynamic Few-Shot Classification → Safety Gate → Query Transformation → RAG Retrieval → Constrained Tool Routing → Grounded Response → Evaluation

- **Problem: ** administrative healthcare requests mix intent recognition, policy lookup, and actions.
- **Solution: ** dynamic few-shot intent classification → safety gate/query transformation → FAISS RAG → constrained tool routing → grounded synthesis.

## Techniques Used and Why They Were Chosen
- Structured/grounded prompting and evaluation discipline/**From Week 3**/Guides the LLM to produce consistent, policy-grounded responses without unsupported medical advice.

- Constrained tool use, validation, routing, and logs/**From Week 4**/Uses validated inputs and predefined tools to ensure safe and controlled administrative workflows
- FAISS RAG with normalized sentence-transformer embeddings/**From Week 5**/Retrieves relevant healthcare policies using semantic embeddings to reduce hallucinations and support evidence-based responses
- Selective query transformation and retrieval analysis/**From Week 6**/Reformulates unclear or incomplete requests to improve retrieval accuracy.
- Dynamic few-shot retrieval for healthcare administrative intent classification/**From Week 7**/Classifies patient requests using similar labeled examples to improve intent recognition.

- **Evaluation: ** 15 held-out cases with intent accuracy, macro-F1, routing accuracy, Recall@3, MRR, and an LLM-as-judge scoring correctness, grounding, and safety/scope.
