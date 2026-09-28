# Luke Bransby

**MSc Data Science & Machine Learning (Distinction) @ UCL** | **BSc Mathematics & Computer Science (First Class) @ QMUL**  
Building production services: a live GB electricity-demand forecast, and a non-diagnostic Crohn’s brief from messy daily logs.

[LinkedIn](https://www.linkedin.com/in/luke-bransby) • [GitHub](https://github.com/lbransby1) • luke.bransby15@gmail.com

---

### Current projects

<table>
  <tr>
    <td width="60%" valign="top">
      <h2><a href="https://grid-demand.uk">Grid Demand UK</a></h2>
      <strong>Live GB National Demand forecast, scored after the fact</strong>
      <ul>
        <li><strong>Product:</strong> Weather in, P10 / P50 / P90 out. Three clocks: next half-hour, midnight day freeze, Monday week freeze. Official outturn (Elexon INDO) is joined only after each settlement period ends.</li>
        <li><strong>Engineering:</strong> FastAPI with a fast read path (<code>GET /board</code> is local parquet only) and forecasts on a background thread. Atomic INDO cache, DST-safe settlement timestamps, pytest + GitHub Actions, Docker on Railway.</li>
        <li><strong>Honesty:</strong> Yesterday on the chart is actuals, not a hindcast. Width is the average blue-band over the whole issued fan; MAE and coverage use only finished half-hours.</li>
      </ul>
      <a href="https://grid-demand.uk">Live site →</a> | <a href="https://github.com/lbransby1/energy-forecast">Source →</a>
    </td>
    <td width="40%" valign="center">
      <img src="https://raw.githubusercontent.com/lbransby1/energy-forecast/main/docs/live-day-board.png" alt="Grid Demand UK: yesterday INDO then today's forecast fan" style="border-radius: 8px; border: 1px solid #30363d;">
    </td>
  </tr>

  <tr>
    <td width="60%" valign="top">
      <h2><a href="https://crohns-care.app">Crohn’s Care</a></h2>
      <strong>Harvey-Bradshaw briefs from unstructured daily logs — not a diagnostic tool</strong>
      <ul>
        <li><strong>Problem:</strong> Patients keep messy diaries (slang, skipped days, fragments). A 10-minute GI slot cannot absorb the raw notes.</li>
        <li><strong>Pipeline:</strong> Instructor + Pydantic extract HBI fields; Python does the arithmetic (windows, adherence, Bristol 6–7 only). Ephemeral Chroma RAG retrieves dated spans so the narrative is cited, not a full-diary dump.</li>
        <li><strong>Ship:</strong> FastAPI, Matplotlib trajectory, one-page ReportLab PDF. Synthetic extraction benchmark (not clinician-labelled real diaries). Guardrails: no drug/diet/referral advice; diaries stay in-request.</li>
      </ul>
      <a href="https://crohns-care.app">Live app →</a> | <a href="https://github.com/lbransby1/crohns-care">Source →</a>
    </td>
    <td width="40%" valign="center">
      <img src="https://github.com/lbransby1/lbransby1/blob/main/crohnsgif.gif" alt="Crohn's Care demo" style="border-radius: 8px; border: 1px solid #30363d;">
    </td>
  </tr>
</table>

---

### Other work

<table>
  <tr>
    <td width="60%" valign="top">
      <h2><a href="https://huggingface.co/spaces/lukebransby/skin-lesion-counterfactual-demo">Skin lesion counterfactuals</a></h2>
      <strong>MSc thesis — explainable edits for clinical dermatology</strong>
      <ul>
        <li>Classifier-free Flow Matching vs latent diffusion; 7-point checklist oracle; InstaFlow for sub-2s inference.</li>
      </ul>
      <a href="https://huggingface.co/spaces/lukebransby/skin-lesion-counterfactual-demo">Demo →</a> | <a href="https://github.com/lbransby1/msc-thesis">Source →</a>
    </td>
    <td width="40%" valign="center">
      <img src="https://github.com/lbransby1/lbransby1/blob/main/lesion.gif" alt="Skin lesion counterfactual demo" style="border-radius: 8px; border: 1px solid #30363d;">
    </td>
  </tr>
  <tr>
    <td width="60%" valign="top">
      <h2><a href="https://m5forecasting.info">M5Forecasting.info</a></h2>
      Quantile LightGBM retail demand, Polars + Redis + FastAPI on Railway.
      <br><a href="https://github.com/lbransby1/M5-Forecasting">Source →</a>
    </td>
    <td width="40%" valign="center">
      <img src="https://raw.githubusercontent.com/lbransby1/M5-Forecasting/832b2211cd305b5034f34cde4fa2f5dd3bd75f35/images/m5-demo.gif" alt="M5 Forecasting demo" style="border-radius: 8px; border: 1px solid #30363d;">
    </td>
  </tr>
  <tr>
    <td width="60%" valign="top">
      <h2><a href="https://fightcast.app">FightCast.app</a></h2>
      MMA outcomes: stacked ensembles and Siamese nets; FastAPI + Streamlit.
      <br><a href="https://github.com/lbransby1/end-to-end-ufc-prediction">Source →</a>
    </td>
    <td width="40%" valign="center">
      <img src="https://github.com/lbransby1/lbransby1/blob/main/MMAMetrics.gif?raw=true" alt="FightCast demo" style="border-radius: 8px; border: 1px solid #30363d;">
    </td>
  </tr>
</table>

---

### Technical skills

* **Languages:** Python, SQL, Bash, R
* **ML / AI:** LightGBM, quantile regression, PyTorch, Flow Matching, SHAP
* **LLM / RAG:** Instructor, Pydantic, ChromaDB, structured extraction, eval harnesses
* **Backend / ops:** FastAPI, Docker, GitHub Actions, pytest, Railway, GCP
