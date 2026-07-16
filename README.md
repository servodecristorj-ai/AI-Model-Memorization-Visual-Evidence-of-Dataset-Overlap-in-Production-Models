umae # AI-Dataset-Overlap: Analyzing Memorization in Meta AI, Gemini & ChatGPT
> **Technical Case Study on Model Overfitting and Shared Training Data in Text-to-Image Generators.**
---
## 📌 Abstract
This repository contains the analysis and empirical evidence of **dataset overlap and model memorization** across state-of-the-art text-to-image AI models (specifically Meta AI and Google Gemini). By utilizing a highly specific, complex prompt, we demonstrated a **>90% structural and conceptual similarity** between competing production models. 
While traditional AI Bug Bounty programs currently classify model training overlaps as *"out of scope"* (as experienced during our disclosure process with Meta and OpenAI), this paper argues that such behavior serves as visible proof of training data replication, bringing forth significant implications for copyright compliance and AI safety.
📄 **[Download the Full Technical Paper (PDF)](./seu-arquivo.pdf)** *(Substitua "seu-arquivo.pdf" pelo nome exato do PDF que você baixou do Overleaf e subiu no repositório)*
---
## 📸 The Experiment & Prompt
The following prompt was executed across five major production models in **July 2026**:
> *"A dramatic Wild West scene at sunset. A cowboy riding a horse made of glowing computer circuit boards and binary code. The horse is rearing up on its hind legs."*
### The "Twin" Generations: Meta AI vs. Google Gemini
Despite the complexity of the prompt, **Meta AI** and **Google Gemini** converged on an almost identical spatial layout:
* **Identical Horse Pose:** Same angle (left profile), same rearing posture, and identical leg anatomy.
* **The Cowboy:** Same leather duster coat, hat shape, and facial profile/lighting.
* **Background Assets:** Matching placement of the *Monument Valley* rock formations under a crimson sky.
* **Face Overlap (Meta vs. ChatGPT):** Structural similarity in facial features, suggesting a shared high-weight vector for "rugged cowboy."
---
## 📊 Comparison Matrix

| Model | Artistic Path | Spatial Layout | Overlap Detected? |
| :--- | :--- | :--- | :--- |
| **Meta AI** | Sci-Fi / Realist | Left Profile (Rearing) | **Yes** (High overlap with Gemini) |
| **Google Gemini** | Sci-Fi / Realist | Left Profile (Rearing) | **Yes** (High overlap with Meta) |
| **ChatGPT (DALL·E 3)** | High-Contrast / Symbolic | Right Profile (Rearing/Gun) | No (Unique artistic interpretation) |
| **Grok** | Cinematic / Neon | Right Profile | No (Unique artistic interpretation) |
| **Dola AI** | Synthwave / Vector | Left Profile | No (Unique artistic interpretation) |

---
## 🛠️ How to Cite this Research
If you find this analysis useful for your research in AI security, memorization, or dataset auditing, please cite it as:
```bibtex
@techreport{servo2026memorization,
  author      = {Servo, Marco},
  title       = {Visual Proof of Model Memorization: A Comparative Case Study of Dataset Overlap in Meta AI and Google Gemini},
  institution = {GitHub Research Group},
  year        = {2026},
  month       = {July},
  url         = {[https://github.com/SEU-USUARIO/NOME-DO-REPOSITORIO](https://github.com/SEU-USUARIO/NOME-DO-REPOSITORIO)}
}
