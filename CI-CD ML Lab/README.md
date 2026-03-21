🤖 CI/CD Pipeline for Machine Learning
📌 Overview

This project demonstrates the implementation of a complete CI/CD pipeline for a Machine Learning system, covering the entire lifecycle from:

➡️ Model Training → Validation → Deployment → Monitoring → Retraining

Unlike traditional software systems, machine learning pipelines are dynamic and data-dependent, requiring continuous validation and monitoring to maintain performance.

This lab focuses on building a production-ready ML pipeline with automation, reliability, and feedback mechanisms.

📂 Project Contents
📓 Swetha_CICD ML Lab.ipynb → Implementation of the ML pipeline
📄 Swetha_CICD ML Lab Report.pdf → Detailed explanation of concepts and workflow
⚙️ Python scripts (logical stages):
train.py
validate.py
drift_detect.py
monitor.py
CI/CD configuration (GitHub Actions)
⚙️ Pipeline Architecture
🔹 1. Training Pipeline (train.py)
Uses the Iris dataset
Splits data into training and testing sets
Trains a Random Forest model
Stores:
Model artifacts
Performance metrics
Configuration
Data hash

📌 Key Concept:
Data versioning ensures reproducibility and helps track changes across runs.

🔹 2. Validation Pipeline (validate.py)

Acts as a quality control stage before deployment.

✔ Includes 4 validation gates:

Schema validation
Performance validation (accuracy, F1-score)
Regression check (compare with previous model)
Fairness validation

➡️ Only models that pass all checks proceed further

🔹 3. Drift Detection (drift_detect.py)
Detects changes in data distribution over time
Uses:
PSI (Population Stability Index)
KL Divergence

📌 Purpose:
Identify when model performance may degrade due to changing data

🔹 4. Continuous Integration (CI)
Implemented using GitHub Actions
Triggered on:
Code changes
Data updates
Scheduled runs

✔ Ensures:

Automated training
Automated validation
Version tracking using commit SHA
🔹 5. Continuous Deployment (CD)
Uses Canary Deployment Strategy

✔ Process:

Deploy to a small subset of users
Monitor performance (accuracy, latency)
Promote or rollback automatically
🔹 6. Production Monitoring (monitor.py)
Continuously tracks:
Model accuracy
Data drift

✔ Features:

Automatic retraining trigger
Circuit breaker to prevent excessive retraining
⚠️ Issues Faced & Resolutions
🔸 CI Pipeline Validation Failure
Issue: Incorrect path filters
Fix: Used exact patterns (src/**, data/**) instead of generic ones
🔸 YAML Formatting Errors
Issue: Pipeline failed due to formatting
Fix: Used block format:
run: |
  command here
🔸 UI vs Terminal Mismatch
Issue: Terminal showed success but UI failed
Insight: Systems validate based on expected structure, not just execution
🔸 Understanding Drift Metrics
Challenge: PSI and KL divergence were initially unclear
Learning: Higher PSI indicates higher data shift → retraining needed
🧠 Key Learnings
ML systems require a continuous lifecycle approach
Validation is essential before deployment
Monitoring ensures long-term reliability
Automation improves consistency and scalability
🚀 How to Run
Install required Python libraries
Run pipeline stages:
python train.py
python validate.py
python drift_detect.py
python monitor.py
Configure CI/CD using GitHub Actions
📈 Skills Demonstrated
💡 Machine Learning
Model training & evaluation
Performance validation
💡 MLOps
CI/CD pipeline design
Drift detection
Monitoring & retraining
💡 Engineering
Automation workflows
Debugging CI/CD pipelines
YAML configuration handling
👩‍💻 Author

Swetha Battula

⭐ Conclusion

This project demonstrates how to build a robust and production-ready machine learning system by integrating:

➡️ Training
➡️ Validation
➡️ Deployment
➡️ Monitoring

It highlights the importance of continuous feedback loops in maintaining reliable ML systems.
