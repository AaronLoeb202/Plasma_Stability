{\rtf1\ansi\ansicpg1252\cocoartf2709
\cocoatextscaling0\cocoaplatform0{\fonttbl\f0\fswiss\fcharset0 Helvetica;}
{\colortbl;\red255\green255\blue255;}
{\*\expandedcolortbl;;}
\paperw11900\paperh16840\margl1440\margr1440\vieww11520\viewh8400\viewkind0
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0

\f0\fs24 \cf0 #  Plasma Disruption Prediction using XGBoost\
\
This project aims to predict plasma disruptions in tokamak experiments using a machine learning model trained on the DB4v5 confinement dataset.  \
We used SHAP for model explainability and performed feature selection to optimize both performance and interpretability.\
\
---\
\
##  Project Structure\
\
- `PlasmaStabilityProject.ipynb` \'97 Jupyter Notebook containing the full data processing, modeling, and SHAP analysis pipeline.\
- `requirements.txt` \'97 List of Python dependencies for reproducibility.\
- `HDB5V2.3.xlsx` \'97 Sample of the cleaned dataset (optional, can be ignored from Git tracking if needed).\
\
---\
\
##  Model Overview\
\
- **Model:** XGBoost Classifier  \
- **Goal:** Predict whether a plasma shot is stable (`STD3 = 0`) or disrupted (`STD3 = 1`)  \
- **Techniques used:**\
  - Feature selection with SHAP  \
  - Cross-validation (F1-score)  \
  - Model simplification with top 20 features  \
  - Model interpretation with SHAP beeswarm plots  \
\
---\
\
##  Key Results\
\
- Achieved **F1-score \uc0\u8776  1.00** on both the full and reduced models  \
- Identified top features like `SELDB3`, `SELDB5`, and `DATE` as key drivers of disruption  \
- Built a lightweight and interpretable model without loss in performance  \
\
---\
\
##  Data Source\
\
This project uses data from the **International H-Mode Confinement Database (DB4v5)**, available via:\
\
> **The International Tokamak Physics Activity (ITPA) Global H-Mode Confinement Database**  \
> Princeton Plasma Physics Laboratory  \
> http://arks.princeton.edu/ark:/88435/dsp01m900nx49h\
\
---\
\
## Installation\
\
To install the dependencies:\
\
```bash\
pip install -r requirements.txt \
```\
Then launch the notebook:\
\
```bash\
jupyter notebook PlasmaStabilityProject.ipynb \
``` \
\
---\
\
##  Author\
\
**Aaron Loeb**  \
Machine Learning & Physics Enthusiast  \
[LinkedIn](https://www.linkedin.com/)\
}