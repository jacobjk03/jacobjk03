# Hi, I'm Jacob Kuriakose 👋
**Data Scientist & Machine Learning Engineer** | *MS in Data Science @ Arizona State University (GPA: 4.0)*

I specialize in building production-grade Machine Learning systems, with a focus on **GenAI (Agentic RAG)**, **MLOps**, and **Cloud Infrastructure**.

---

### 🚀 High-Impact Engineering
* **Cloud & MLOps:** Led the migration of a production-grade AI chatbot to **AWS**, improving deployment efficiency by **~85%** and reducing manual setup by **~40%** using **AWS CDK**.
* **Generative AI:** Engineered an agentic **Medical Chatbot** featuring a **ReAct** architecture with **MedGemma** and **LLaMA-3**, achieving a $F1 \approx 0.84$ for factual grounding and a **1.0 Safety score**.
* **Time Series & Forecasting:** Optimized Walmart sales predictions, achieving a **38.92% RMSE improvement** using Exponential Smoothing; integrated **MLflow** and **DVC** for full experiment tracking.

---

### 📂 Featured Projects

#### 👤 Personal Projects (GenAI & Data Science)
* **[Medical Agentic RAG](https://github.com/jacobjk03/Medical_chatbot):** A GenAI system using hybrid LLM orchestration (MedGemma + LLaMA-3) and LangGraph to provide factually grounded medical reasoning.

```mermaid
graph TD
    A[User Query] --> B{Agentic Router}
    B -->|Medical Query| C[Pinecone Vector Search]
    B -->|General/Recent| D[Web Search Tool]
    C --> E[Cross-Encoder Reranker]
    E --> F[MedGemma / LLaMA-3 LLM]
    D --> F
    F --> G[Thought: Reasoning Chain]
    G --> H[Action: Tool Call]
    H --> I[Observation: Context]
    I --> J{Sufficient Info?}
    J -->|No| G
    J -->|Yes| K[Final Answer with Disclaimers]
```

* **[Walmart Sales Pipeline](https://github.com/jacobjk03/Data-Driven-Walmart-Sales-Predictions):** An end-to-end forecasting project featuring SARIMA/LSTM models, **MLflow** for tracking, and **DVC** for data versioning.

```mermaid
graph LR
    Data[(Raw Data)] --> DVC[DVC Versioning]
    DVC --> Train[Model Training: LSTM/SARIMA]
    Train --> MLflow[MLflow Experiment Tracking]
    MLflow --> Best[Best Model Selection]
    Best --> API[FastAPI Deployment]
    API --> Pred[Sales Forecasts]
```

#### 👥 Team Projects (GenAI, MLOps & Software Dev)
* **[Waterbot (AWS Migration)](https://github.com/jacobjk03/waterbot/tree/main):** Led the transition of this AI chatbot to a CISA-compliant AWS stack (ECS, Lambda, Bedrock), slashing release times by **85%**.

```mermaid
graph TD
    User((User)) --> CF[CloudFront]
    CF --> ALB[Load Balancer]
    ALB --> ECS[ECS on Fargate]
    subgraph AWS_CISA_Infrastructure[AWS CISA Infrastructure]
    ECS --> Bedrock[Amazon Bedrock Knowledge Base]
    ECS --> S3[S3 Assets]
    ECS --> DB[(DynamoDB)]
    end
    CDK[AWS CDK] -->|IaC Provisioning| AWS_CISA_Infrastructure
```

* **[Navia](https://github.com/jacobjk03/Navia):** An end-to-end product integrating GenAI capabilities with full-stack software development to solve real-world user needs.

```mermaid
graph LR
    UI[React Frontend] --> Vercel[Hosted on Vercel]
    Vercel --> API[TypeScript Backend]
    API --> Agent[Agentic AI Chatbot]
    Agent --> LLM[LLM Orchestration]
```

---

### 🛠️ Technical Toolkit
* **AI/ML:** TensorFlow, PyTorch, LangChain, LangGraph, Hugging Face, Time Series, Vector DBs (Pinecone, Bedrock).
* **Infrastructure:** AWS (ECS, ECR, Lambda, CDK), Docker, FastAPI, MLflow, DVC.
* **Languages:** Python (NumPy, Pandas, Scikit-learn), SQL, C++, GoLang.

---

📫 **Connect with me:** [LinkedIn](https://www.linkedin.com/in/jacob-kuriakose) | [Portfolio Website](https://www.jacobkuriakose.com/)
