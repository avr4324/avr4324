<h1 align="center">Aditya Vardhan Reddy</h1>

<p align="center">
  <b>Software Engineer · AI/ML · Retrieval and Explainability</b>
</p>

<p align="center">
  <a href="https://github.com/avr4324">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=20&pause=1300&color=4FC3F7&center=true&vCenter=true&width=740&lines=Software+Engineer+%40+Viasat+%E2%80%94+cloud+data+platforms;Building+and+evaluating+RAG+systems;Published+on+bias+%26+interpretability+of+deep+learning;Applying+for+MS+CS+(AI%2FML)+%E2%80%94+Fall+2027" alt="Typing intro">
  </a>
</p>

<p align="center">
  <a href="https://linkedin.com/in/aditya-vardhan-reddy-a68822273"><img src="https://img.shields.io/badge/LinkedIn-connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="https://doi.org/10.1007/978-3-032-06694-7_46"><img src="https://img.shields.io/badge/Springer-LNNS%202025-EA4F2B?style=for-the-badge" alt="Springer paper"></a>
  <img src="https://img.shields.io/badge/Hyderabad-India-555555?style=for-the-badge" alt="Hyderabad, India">
  <img src="https://komarev.com/ghpvc/?username=avr4324&label=Profile%20views&color=2c5364&style=for-the-badge" alt="Profile views">
</p>

I build cloud data governance and logging infrastructure on GCP at Viasat. Outside work I build AI systems and test them properly. I care about showing that a model or pipeline works, with evaluation, not just running it. I'm preparing to start an MS in Computer Science (AI/ML) in Fall 2027.

---

##  At a glance

<table align="center">
  <tr>
    <td align="center"><h3>8.72 / 10</h3><sub>B.Tech CGPA<br>Computer Science and AI</sub></td>
    <td align="center"><h3>1</h3><sub>Springer<br>publication</sub></td>
    <td align="center"><h3>0.58 → 0.62</h3><sub>nDCG@10 gain<br>from hybrid retrieval</sub></td>
    <td align="center"><h3>68.7% → 78.2%</h3><sub>accuracy gain from<br>Bias-Aware Grad-CAM</sub></td>
  </tr>
</table>

##  Journey

```mermaid
timeline
    title From B.Tech to MS
    2021 : B.Tech in CS and AI begins at Amrita
    2024 : Research Intern at UC Santa Cruz (Tech4Good Lab)
    2025 : Software Engineer Intern at Viasat (Jan)
         : Springer LNNS paper published
         : B.Tech completed (May)
         : Software Engineer 1 at Viasat (Jul)
    2027 : MS in Computer Science, AI/ML (planned)
```

##  Projects

### Corrective RAG Engine
`LangGraph` `FastAPI` `Qdrant` `Streamlit` `Docker Compose`

A RAG system that checks its own retrieval before answering. It scores whether the retrieved context is relevant, rewrites the query when it isn't, and evaluates answer faithfulness and retrieval relevance.

```mermaid
flowchart LR
    A([User query]) --> B[Hybrid retrieval<br>Qdrant]
    B --> C{Is the context<br>relevant?}
    C -- Yes --> D[Generate answer]
    C -- No --> E[Rewrite query]
    E --> B
    D --> F([Evaluate faithfulness<br>and retrieval relevance])
```

### Incident Summarizer with Retrieval and Evaluation
`Python` `scikit-learn` `sentence-transformers`

Finds similar past outages and drafts a likely cause and fix, citing the incidents it used.

| | |
|---|---|
| **Compared** | BM25, TF-IDF, LSA, dense (MiniLM), hybrid |
| **Setup** | 100 labeled public post-mortems, leave-one-out, bootstrap confidence intervals |
| **Finding** | A BM25 + dense hybrid gave a small but reliable nDCG@10 gain over BM25 (0.58 → 0.62). Dense alone did not. |

### [Alzheimer's Disease Prediction](https://github.com/avr4324/ALZHEIMER-S-DISEASE-PREDICTION-USING-TRANSFER-LEARNING-AND-CNN)
`TensorFlow` `Keras` `InceptionV3`

A CNN with transfer learning that classifies brain MRI scans into four dementia stages, reaching 80.47% test accuracy and 81.30% validation AUC.

## 🔬 Research

**[Exploring Biases and Interpretability of Deep Learning Models](https://doi.org/10.1007/978-3-032-06694-7_46)**, Springer LNNS, 2025
A Bias-Aware Grad-CAM framework for ResNet race and gender classifiers on UTKFace. It measures how well the model's attention matches facial regions (IoU) and feeds that back into the loss, raising test accuracy from 68.7% to 78.2%.

**Research Intern, Tech4Good Lab, UC Santa Cruz**, summer 2024
AI-assisted ideation: detecting idea saturation and improving human-AI brainstorming through constraint-based prompting.

## 🛠 Skills

<p>
  <img src="https://skillicons.dev/icons?i=python,java,js,tensorflow,sklearn,fastapi,django,docker,terraform,ansible,gcp,aws,githubactions,linux,git&perline=8" alt="Tech stack">
</p>

**Data:** BigQuery · Snowflake · Snowplow · Airflow · SQL

---

<p align="center">
  <a href="https://linkedin.com/in/aditya-vardhan-reddy-a68822273">LinkedIn</a>
  &nbsp;·&nbsp;
  <a href="https://doi.org/10.1007/978-3-032-06694-7_46">Publication</a>
</p>