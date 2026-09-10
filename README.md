# Luke Bransby

**MSc Data Science & Machine Learning (Distinction) @ UCL** | **BSc Mathematics & Computer Science (First Class) @ QMUL**  
Specialising in deterministic LLM systems, probabilistic time-series forecasting, and generative computer vision.

[LinkedIn](https://www.linkedin.com/in/luke-bransby) • [GitHub](https://github.com/lbransby1) • luke.bransby15@gmail.com

---

### Featured Projects & Deployed Systems

<table>
  <tr>
    <td width="60%" valign="top">
      <h2><a href="https://huggingface.co/spaces/lukebransby/skin-lesion-counterfactual-demo">Skin Lesion Counterfactual Generation</a></h2>
      <strong>Explainable AI for Clinical Dermatology (MSc Thesis)</strong>
      <ul>
        <li><strong>Research:</strong> Formulated classifier-free <strong>Flow Matching</strong> to generate counterfactual dermoscopy edits flipping an ensemble clinical oracle. Proved Flow Matching reduces hallucinated artifacts over Latent Diffusion.</li>
        <li><strong>Evaluation:</strong> Assessed via a decoupled 7-head clinical oracle mimicking the dermatological 7-point checklist; evaluated directional edit metrics ($\Delta\text{Checklist}$, SSIM, LPIPS) alongside cycle-reversibility.</li>
        <li><strong>Inference:</strong> Integrated <strong>InstaFlow</strong> for sub-2s inference on consumer hardware. Manuscript targeting AIME 2027.</li>
      </ul>
      <a href="https://huggingface.co/spaces/lukebransby/skin-lesion-counterfactual-demo">Live Demo (Hugging Face) →</a> | <a href="https://github.com/lbransby1/msc-thesis">View Source Code →</a>
    </td>
    <td width="40%" valign="center">
      <img src="https://huggingface.co/spaces/lukebransby/skin-lesion-counterfactual-demo/raw/main/thumbnail.png" alt="Skin Lesion Counterfactual Demo" style="border-radius: 8px; border: 1px solid #30363d;" onerror="this.src='https://raw.githubusercontent.com/lbransby1/lbransby1/main/assets/thesis-placeholder.png';">
    </td>
  </tr>

  <tr>
    <td width="60%" valign="top">
      <h2>Crohn’s Care: Grounded Clinical Briefs with RAG</h2>
      <strong>Deterministic Health Logging & Non-Diagnostic Decision Support</strong>
      <ul>
        <li><strong>Deterministic Extraction:</strong> Maps unstructured, colloquial daily symptom diaries to structured Harvey-Bradshaw Index (HBI) fields using <strong>Instructor + Pydantic</strong>; computes trajectory windows and arithmetic entirely in deterministic Python.</li>
        <li><strong>Ephemeral RAG:</strong> Builds per-request <strong>Chroma</strong> indices with temporal metadata tagging, preventing full context dumps while ensuring citations reflect exact event spans.</li>
        <li><strong>System Architecture:</strong> Containerised <strong>FastAPI</strong> microservice generating dynamic trajectory visualisations (Matplotlib) and exportable one-page clinical PDF briefs (ReportLab).</li>
      </ul>
      <a href="https://github.com/lbransby1/crohns-care">View Source Code →</a>
    </td>
    <td width="40%" valign="center">
      <img src="https://raw.githubusercontent.com/lbransby1/lbransby1/main/assets/crohns-demo.png" alt="Crohns Care Architecture Demo" style="border-radius: 8px; border: 1px solid #30363d;" onerror="this.src='https://raw.githubusercontent.com/lbransby1/lbransby1/main/assets/rag-placeholder.png';">
    </td>
  </tr>

  <tr>
    <td width="60%" valign="top">
      <h2><a href="https://m5forecasting.info">M5Forecasting.info</a></h2>
      <strong>High-Throughput Probabilistic Retail Demand Forecasting</strong>
      <ul>
        <li><strong>The Problem:</strong> Quantifying inventory safety stock across multi-echelon retail hierarchies under intermittent demand.</li>
        <li><strong>Modelling:</strong> Multi-quantile <strong>LightGBM</strong> pipelines optimized with <strong>Weights & Biases</strong>; zero-shot SHAP explanations for human interpretability.</li>
        <li><strong>Production Engineering:</strong> <strong>Polars</strong> data engine with <strong>Redis</strong> dataset caching and a <strong>FastAPI</strong> backend deployed to Railway for sub-second inference.</li>
      </ul>
      <a href="https://github.com/lbransby1/M5-Forecasting">View Source Code →</a>
    </td>
    <td width="40%" valign="center">
      <img src="https://raw.githubusercontent.com/lbransby1/M5-Forecasting/832b2211cd305b5034f34cde4fa2f5dd3bd75f35/images/m5-demo.gif" alt="M5 Forecasting Demo" style="border-radius: 8px; border: 1px solid #30363d;">
    </td>
  </tr>

  <tr>
    <td width="60%" valign="top">
      <h2><a href="https://fightcast.app">FightCast.app</a></h2>
      <strong>MMA Predictive Analytics & Upset Detection</strong>
      <ul>
        <li><strong>Modelling:</strong> Combat sports outcome forecasting using Ensemble Stacking and Siamese Neural Networks to eliminate corner bias.</li>
        <li><strong>Stack:</strong> Dockerized web platform powered by <strong>FastAPI</strong> and <strong>Streamlit</strong>, featuring real-time matchup metrics and attribute radar charts.</li>
      </ul>
      <a href="https://github.com/lbransby1/end-to-end-ufc-prediction">View Source Code →</a>
    </td>
    <td width="40%" valign="center">
      <img src="https://github.com/lbransby1/lbransby1/blob/main/MMAMetrics.gif?raw=true" alt="FightCast Demo" style="border-radius: 8px; border: 1px solid #30363d;">
    </td>
  </tr>
</table>

---

### Technical Skills

* **Languages & Core:** Python (Expert), SQL, Bash, R
* **Machine Learning & AI:** PyTorch, LightGBM, Flow Matching, Latent Diffusion, Quantile Regression, Bayesian Optimization, XAI (SHAP, Counterfactuals)
* **LLM Engineering & RAG:** Instructor, Pydantic, ChromaDB, Structured Extraction, Context Construction, Evaluation Harnesses
* **Data & Backend Engineering:** FastAPI, Polars, PySpark, Redis, Docker, GCP (GKE, Cloud Run), GitHub Actions (CI/CD), PyTest
