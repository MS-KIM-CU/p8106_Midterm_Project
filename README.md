# P8106 Midterm Project

Prediction model for log-transformed progression-free survival (PFS) in breast cancer patients.

## Repository Structure

```
├── data/
│   ├── datA.RData          # Cohort A (1990–1995, n = 2000)
│   └── datB.RData          # Cohort B (2000–2005, n = 2000)
├── figures/                 # Auto-generated plots from Rmd knitting
├── Midterm_EDA.Rmd          # EDA & data cleaning
└── README.md
```

## Data

| Variable | Column | Description |
|---|---|---|
| Age | `age` | Age at diagnosis (years) |
| Menopausal status | `menopause` | 0 = Pre, 1 = Post |
| Race/ethnicity | `race` | 1 = White, 2 = Black, 3 = Asian, 4 = Hispanic |
| BMI | `bmi` | Body Mass Index at diagnosis (kg/m²) |
| Tumor size | `tumor_size` | Tumor size at diagnosis (cm) |
| Tumor grade | `tumor_grade` | 1 = Well, 2 = Moderate, 3 = Poorly differentiated |
| Positive lymph nodes | `lymph_nodes` | Number of positive axillary lymph nodes |
| ER status | `ER` | 0 = Negative, 1 = Positive |
| PR status | `PR` | 0 = Negative, 1 = Positive |
| HER2 status | `HER2` | 0 = Negative, 1 = Positive |
| Ki-67 index | `Ki67` | Ki-67 proliferation index (%) |
| Clinical stage | `stage` | 1 = Stage I, 2 = Stage II, 3 = Stage III |
| Surgery type | `surgery` | 0 = Breast-conserving, 1 = Mastectomy |
| Chemotherapy | `chemo` | 0 = No, 1 = Yes |
| Hormonal therapy | `hormonal_therapy` | 0 = No, 1 = Yes |
| **log(PFS)** | `log_PFS` | **Response** — log-transformed PFS (months) |

## How to Run

1. Open `Midterm_EDA.Rmd` in RStudio.
2. Knit to HTML — figures are saved automatically to `figures/`.
