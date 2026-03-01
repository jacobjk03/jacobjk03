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
graph TB
    A[User Query] --> B{Agentic Router}
    B -->|Medical Query| C[Pinecone Vector<br/>Search]
    B -->|General/Recent| D[Web Search<br/>Tool]
    C --> E[Cross-Encoder<br/>Reranker]
    E --> F[MedGemma /<br/>LLaMA-3 LLM]
    D --> F
    F --> G[Thought:<br/>Reasoning Chain]
    G --> H[Action:<br/>Tool Call]
    H --> I[Observation:<br/>Context]
    I --> J{Sufficient<br/>Info?}
    J -->|No| G
    J -->|Yes| K[Final Answer with<br/>Disclaimers]
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

### 🛠️ Technical Toolkit

**Data Science & Machine Learning (Core)**
<p align="left">
  <img src="https://img.shields.io/badge/Scikit_Learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white" />
  <img src="https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white" />
  <img src="https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white" />
  <img src="https://img.shields.io/badge/Matplotlib-ffffff?style=flat-square&logo=matplotlib&logoColor=black" />
  <img src="https://img.shields.io/badge/SciPy-8CAAE6?style=flat-square&logo=scipy&logoColor=white" />
  <img src="https://img.shields.io/badge/XGBoost-232F3E?style=flat-square&logo=xgboost&logoColor=white" />
</p>

**Deep Learning (Computer Vision & NLP)**
<p align="left">
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white" />
  <img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white" />
  <img src="https://img.shields.io/badge/Keras-D00000?style=flat-square&logo=keras&logoColor=white" />
  <img src="https://img.shields.io/badge/Hugging_Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black" />
  <img src="https://img.shields.io/badge/NLTK-154F7B?style=flat-square&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/spaCy-09A3D5?style=flat-square&logo=spacy&logoColor=white" />
  <img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white" />
</p>

**Generative AI & Agentic Systems**
<p align="left">
  <img src="https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=chainlink&logoColor=white" />
  <img src="https://img.shields.io/badge/LangGraph-000000?style=flat-square&logo=langchain&logoColor=white" />
  <img src="https://img.shields.io/badge/LlamaIndex-000000?style=flat-square&logo=llama&logoColor=white" />
  <img src="https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white" />
  <img src="https://img.shields.io/badge/Anthropic-754630?style=flat-square&logo=anthropic&logoColor=white" />
  <img src="https://img.shields.io/badge/Vector_DB-Pinecone-000000?style=flat-square&logo=pinecone&logoColor=white" />
</p>

**Infrastructure & MLOps**
<p align="left">
  <img src="https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazon-aws&logoColor=white" />
  <img src="https://img.shields.io/badge/AWS_CDK-FF9900?style=flat-square&logo=amazon-aws&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" />
  <img src="https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white" />
  <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" />
  <img src="https://img.shields.io/badge/MLflow-0194E2?style=flat-square&logo=mlflow&logoColor=white" />
  <img src="https://img.shields.io/badge/DVC-945DD6?style=flat-square&logo=dvc&logoColor=white" />
  <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=github-actions&logoColor=white" />
</p>

**Languages**
<p align="left">
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=white" />
  <img src="https://img.shields.io/badge/C%2B%2B-00599C?style=flat-square&logo=c%2B%2B&logoColor=white" />
  <img src="https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white" />
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" />
<img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black" />
</p>

---

### 📫 Connect with me
<p align="left">
<a href="https://www.linkedin.com/in/jacob-kuriakose"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
<a href="https://www.jacobkuriakose.com/"><img src="https://img.shields.io/badge/Portfolio_Website-4E4E4E?style=for-the-badge&logo=google-chrome&logoColor=white" /></a>
</p>
