# 🎯 Machine Learning & Computer Vision Portfolio Audit Report (Phase 2 Revision)

**Candidate**: Angel Mishra  
**Target Placement Profile**: Java Backend Developer / Full-Stack Developer  
**Secondary Differentiator**: Machine Learning & Computer Vision Research Exposure (NIT Kurukshetra Internship & Final Year Project)  
**Academic Background**: B.Tech in Electronics & Communication Engineering (ECE), Banasthali Vidyapith  
**GitHub**: [https://github.com/123angmish](https://github.com/123angmish)  

---

## 1. Executive Summary & Verification Standards

This revised audit resolves all remaining methodological and provenance discrepancies, enforcing strict scientific integrity, technical reproducibility, and transparent reporting.

### Core Standards Enforced:
1. **Source Code is Ground Truth**: Removed all unsupported claims, fabricated metric numbers, and mathematically generated training curves.
2. **Proper Model Selection**: Selected Linear Regression ($R^2 = 0.8824$, $\text{RMSE} = 4.5194$) as the best-performing model on the synthetic benchmark dataset because the underlying data generation process is largely linear with additive noise.
3. **Transparent Provenance**: Verified the saved MobileNetV2 architecture in `flood_model.h5` while explicitly documenting that original training dataset provenance was not preserved. Built reproducible dataset loading and retraining modules requiring genuine labeled images in `data/`.
4. **Dynamic CI Badges**: Replaced static status badges with live GitHub Actions workflow URLs.

---

## 2. Detailed Audit & Changes by ML/CV Repository

### A. AI Virality Predictor (`ai-virality-predictor`)
- **Dataset Classification**: Standardized Synthetic Benchmark Dataset ($N=10,000$, Seed `42`) parameterized by controlled synthetic distributions to model plausible feature ranges.
- **Model Selection & Rationale**:
  - **Linear Regression (Selected Baseline)**: $R^2 = 0.8824$, $\text{RMSE} = 4.5194$, $\text{MAE} = 3.7105$
  - **Ridge Regression ($\alpha=1.0$)**: $R^2 = 0.8824$, $\text{RMSE} = 4.5195$, $\text{MAE} = 3.7105$
  - **HistGradientBoosting Regressor (Comparison)**: $R^2 = 0.8669$, $\text{RMSE} = 4.8081$, $\text{MAE} = 3.9141$
  - **Gradient Boosting Regressor (Comparison)**: $R^2 = 0.8651$, $\text{RMSE} = 4.8396$, $\text{MAE} = 3.9203$
  - **Random Forest Regressor (Comparison)**: $R^2 = 0.8007$, $\text{RMSE} = 5.8836$, $\text{MAE} = 4.6765$
- **Artifacts Generated from Selected Model**:
  - `backend/artifacts/predicted_vs_actual.png`
  - `backend/artifacts/residual_distribution.png`
  - `backend/artifacts/feature_importance.png` (Permutation Importance on Linear Regression)
  - `backend/artifacts/coefficient_importance.png` & `coefficient_analysis.json`
  - `backend/artifacts/model_comparison.png` & `model_comparison.json`
- **Environment & Serialization Provenance**:
  - Saved `python_version` (3.10), `scikit_learn_version` (1.4+), and `serialization_method` in `model_metadata.json`.
- **Tests & CI**:
  - Pytest: **9 / 9 passed**.
  - Cleaned `requirements.txt` removing unused libraries (`xgboost`, `datasets`, `kaggle`, `easyocr`).
  - Added real GitHub Actions CI badge.

---

### B. FloodGuard AI (`floodguard-ai`)
- **Removal of Synthetic Image Benchmark & Fabricated Curves**:
  - Removed random synthetic image generation from `training/dataset.py`.
  - Deleted fabricated metrics ($0.54$ accuracy, $0$ precision/recall, $0.0052$ ROC-AUC) and fabricated `training_curves.png`.
- **Verified Saved Model Architecture (`training/inspect_model.py`)**:
  - Saved in `artifacts/model_architecture.json`:
    - MobileNetV2 ImageNet frozen backbone (2,257,984 non-trainable parameters).
    - Head: `GlobalAveragePooling2D` $\rightarrow$ `Dense(128, relu)` $\rightarrow$ `Dropout(0.2)` $\rightarrow$ `Dense(1, sigmoid)` (164,097 trainable parameters).
    - Total Parameters: 2,422,081 (9.24 MB).
- **Dataset Loader & Retraining Pipeline**:
  - `training/dataset.py`: Validates and loads genuine labeled images from `data/train`, `data/val`, and `data/test`.
  - `training/train.py`: Trains MobileNetV2 only when real labeled data is supplied, saving new models to `artifacts/flood_mobilenetv2_retrained.keras` (never overwriting `flood_model.h5`) and plotting actual curves only from `history.history`.
  - `training/evaluate.py`: Evaluates held-out performance only when real labeled test data exists.
  - `tests/fixtures/synthetic_test_tensors.py`: Mock tensors scoped strictly for unit test execution without making performance claims.
- **Tests & CI**:
  - Pytest: **9 / 9 passed**.
  - Switched to `opencv-python-headless` and streamlined `.github/workflows/ci.yml`.
  - Added real GitHub Actions CI badge.

---

## 3. Interview Guidelines & Defensibility

### What to SAY in Interviews
- **Primary Focus**: "My primary profile is Java backend and full-stack engineering with Spring Boot, Spring Security, React, and PostgreSQL. In addition, I have hands-on research and applied experience in Machine Learning and Computer Vision."
- **AI Virality Predictor**: "The project started as a Flask research prototype during my internship at NIT Kurukshetra focusing on OpenCV optical flow and Librosa audio analysis. Later, I expanded it into a full-stack platform using FastAPI and Next.js 14. On our synthetic benchmark comparison, Linear Regression achieved the best performance ($R^2 = 0.8824$) because the engineered target is largely linear, demonstrating why simpler models should be chosen when supported by experimental evidence."
- **FloodGuard AI**: "For my final year B.Tech ECE project, I developed an end-to-end prototype combining MobileNetV2 transfer learning for flood scene classification with Lucas-Kanade optical flow for relative surface motion tracking, broadcasting real-time alerts via WebSockets."

### What NOT to Say
- ❌ Do NOT claim you trained models on millions of live scraped YouTube accounts.
- ❌ Do NOT claim optical flow measures exact municipal-grade water velocity without camera calibration.
- ❌ Do NOT claim high model accuracy on FloodGuard AI unless evaluated on a genuine labeled benchmark dataset.