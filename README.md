# Corporate Knowledge Assistant via RAG Architecture 📚

A production-grade Retrieval-Augmented Generation (RAG) system engineered to eliminate hallucinations in conversational AI. This workspace hooks up an LLM directly to a specialized vector database containing an internal corporate handbook, enforcing absolute data grounding.

## 🛠️ Architecture & Tech Stack
* **Agent Orchestration Engine:** Dify.ai (Chatflow Node Canvas)
* **Knowledge Infrastructure:** High-Quality Vector Embeddings & Segmentation Chunking
* **Design Pattern:** Prompt Grounding & Strict Fallback Triage Boundaries

## 🧠 Structural Core
1. **User Intake:** Captures user queries directly through a dynamic conversational node.
2. **Knowledge Retrieval Engine:** Runs the input string query through a Vector Database dataset layer to extract matching content chunks.
3. **Context Injection:** Feeds the isolated source text chunks directly into the LLM prompt's runtime context variable (`{{context}}`).
4. **Guardrailed Inference:** Evaluates the question using *only* the retrieved boundaries, executing a hard-coded fallback refusal message if the request sits outside the documentation footprint.

## 📁 How to Import This App
1. Download the blueprint DSL file from this repository.
2. Open your Dify.ai dashboard, click **Create from Blank**, and select **Import DSL / Blueprint**.
3. Upload the file to immediately deploy the full visual RAG node chain!
