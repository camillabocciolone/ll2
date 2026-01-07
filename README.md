# II2 — EEGPT vs Functional Data Analysis (FDA) in low-subject, subject-independent EEG

Questo repository contiene i notebook usati per gli esperimenti del paper **“Comparing EEG Foundation Models and Functional Data Analysis in Low-Subject, Subject-Independent Settings”** :contentReference[oaicite:1]{index=1}.

L’obiettivo è confrontare:
- **EEGPT** (foundation model) → embeddings finestra-livello + classificatore MLP
- **FDA / fPCA** (approcci interpretabili) → feature fPCA (per-canale e globali) + lo stesso MLP

su un dataset EEG con **15 soggetti**, **8 canali**, due task (**Arithmetic** e **Stroop**) e due setting di etichette:
- **4-classi**: `neutral`, `low`, `mid`, `high`
- **2-classi (binary)**: `neutral` vs `task` (low+mid+high)

---

## Contenuto del repository

- `Arithmetic_4classes_eegpt_vs_fda.ipynb`  
  Esperimenti sul task **Arithmetic** in **4-classi**.

- `Arithmetic_2_classi_eegpt_vs_fda.ipynb`  
  Esperimenti sul task **Arithmetic** in **2-classi** (neutral vs task).

- `Stroop_4classes_eegpt_vs_fda.ipynb`  
  Esperimenti sul task **Stroop** in **4-classi**.

- `Stroop_2_classi_eegpt_vs_fda.ipynb`  
  Esperimenti sul task **Stroop** in **2-classi** (neutral vs task).

> Nota: i notebook sono “self-co
