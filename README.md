# Hi, I'm Jacob Kuriakose 👋
**Data Scientist & Machine Learning Engineer** | *MS in Data Science @ Arizona State University (GPA: 4.0)*

I specialize in building production-grade Machine Learning systems, with a focus on **GenAI (Agentic RAG)**, **MLOps**, and **Cloud Infrastructure**.

---

### 🚀 High-Impact Engineering

| Domain | Core Accomplishment | Key Result |
| :--- | :--- | :--- |
| **☁️ Cloud & MLOps** | Migrated production AI chatbot to **AWS** via **AWS CDK** | **85% ↑** Deployment Efficiency |
| **🤖 Generative AI** | Engineered Agentic **Medical Chatbot** (ReAct + LLaMA-3) | **0.84 $F1$** / **1.0 Safety** |
| **📈 Forecasting** | Optimized Walmart Sales predictions via **MLflow & DVC** | **38.92% ↓** RMSE |

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

### 📂 Featured Projects

| 👤 Personal (GenAI & Data Science) | 👥 Team (MLOps & Software Dev) |
| :--- | :--- |
| **[Medical Agentic RAG](https://github.com/jacobjk03/Medical_chatbot)**<br>Hybrid LLM orchestration (MedGemma + LLaMA-3) and LangGraph. | **[Waterbot (AWS Migration)](https://github.com/jacobjk03/waterbot/tree/main)**<br>CISA-compliant AWS stack (ECS, Lambda, Bedrock) with **85% ↑** efficiency. |
| **[Walmart Sales Pipeline](https://github.com/jacobjk03/Data-Driven-Walmart-Sales-Predictions)**<br>End-to-end forecasting with **MLflow** and **DVC**. | **[Navia](https://github.com/jacobjk03/Navia)**<br>Full-stack product integrating GenAI with TypeScript and React. |

---

#### 🏗️ System Architectures

<div align="center">

| 🩺 Medical RAG (Personal) | 🛒 Walmart Pipeline (Personal) |
| :--- | :--- |
| ![Medical Architecture](https://mermaid.ink/img/pako:eNqNkk1LAzEQhv_KMNee9Af0IggVvYigB8GLl-02u002O5uYpS3S_90kXatVvLg8M88775vJpE_SGBMo6M0reS0pB_IsF6vO99m8pAn4B61P5mN69pI1Y0H_vW_MIdvO1G3K_9mXpq0f4yZ_lX77_T_XN0O2H_D8tX_H38hK-zH-vH_L6znbz8m_eN4-pOfv8vRrfz9m--n5m76_9_dzth_x_LV_x9_ISvtx_rx_y-s528_Jv3jePqTn7_L0a38_Zvvp-Zu-v_f38_O62W7X-xM26o_Y) | ![Walmart Pipeline](https://mermaid.ink/img/pako:eNqNkc9KAzEQxl_FmGtP-gN6EYSKXkTQg-DFy3ab3SabnU3M0hbpuyfptFrFi8sz_L7v_DKZDInaHCDozSt5Iyknck_O1m0as3mJB_IP2p_MZ_S8JWtOf9-3-pA9T3Wf8mX-mbm7n9Mof8tfu-_2_7ndDHn9COdf-nf6jdxrN86fdX95M_f6OfUXL9un9LzN7z7312Oun97f6fvLX8-5fnr9pt-v_vWc60c8f-nf6Tdyr904f9b95c3c6-fUX7xsn9LzNr_73F-PuX56f6fvL3895_p5Xbfbx_0JS_U7bPcf8-V32A) |
| 💧 Waterbot AWS (Team) | 🧭 Navia Flow (Team) |
| ![Waterbot AWS](https://mermaid.ink/img/pako:eNqNkc1KAzEQxl_FmGtP-gN6EYSKXkTQg-DFy3ab3SabnU3M0hbpuyfpWq3ixeWZed93_plMhlidBwj68ELeSsqB3MtF2_ke69e0Av-o7cF8QM9BsmbM6G_7xh6y60zf5HzKvzRv_Rh2-Wv-0373v_fbeMjrS7z80r-Tb-SxeR9_3v_k_ZzN5-RfPG8f0vN_8_Rzfx9m-un5m76_8vczm494-dK_k2_ksXkff97_5P2czeXkXzxvH9Lzf_P0c38fZvrp-Zu-v_L3M5uv29u7xw8W6n_Y7L_6hW__AgvbeX0) | ![Navia Flow](https://mermaid.ink/img/pako:eNqNkc1KAzEQxl_FmGtP-gN6EYSKXkTQg-DFy3ab3SabnU3M0hbpuyfpWq3ixeWZed93_plMhlidBwj68ELeSsqB3MtF2_ke69e0Av-o7cF8QM9BsmbM6G_7xh6y60zf5HzKvzRv_Rh2-Wv-0373v_fbeMjrS7z80r-Tb-SxeR9_3v_k_ZzN5-RfPG8f0vN_8_Rzfx9m-un5m76_8vczm494-dK_k2_ksXkff97_5P2czeXkXzxvH9Lzf_P0c38fZvrp-Zu-v_L3M5uv29u7xw8W6n_Y7L_6hW__AgvbeX0) |

</div>

---

---

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

**AI-First Development & IDEs**
<p align="left">
  <img src="https://img.shields.io/badge/Cursor-000000?style=flat-square&logo=cursor&logoColor=white" />
  <img src="https://img.shields.io/badge/Windsurf-1E1E1E?style=flat-square&logo=visual-studio-code&logoColor=007ACC" />
  <img src="https://img.shields.io/badge/VS_Code-007ACC?style=flat-square&logo=visual-studio-code&logoColor=white" />
  <img src="https://img.shields.io/badge/Antigravity-FF4B4B?style=flat-square&logo=rocket&logoColor=white" />
  <img src="https://img.shields.io/badge/Postman-FF6C37?style=flat-square&logo=postman&logoColor=white" />
  <img src="https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white" />
</p>

---

### 📫 Connect with me
<p align="left">
<a href="https://www.linkedin.com/in/jacob-kuriakose"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
<a href="https://www.jacobkuriakose.com/"><img src="https://img.shields.io/badge/Portfolio_Website-4E4E4E?style=for-the-badge&logo=google-chrome&logoColor=white" /></a>
</p>
