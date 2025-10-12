# Iterative CNN Development for Image Classification: From 78% to 90.9% Accuracy

This repository contains a machine learning project showcasing the systematic development of a high-performance image classification model. The project was undertaken as a demonstration of my practical ML skills and problem-solving abilities for the Google internship application.

**The complete methodology, analysis, and results are documented in the full technical report.**

### ➡️ **[View the Full Technical Report (PDF)](report/project_report.pdf)**

---

## Final Model Performance

The final model, achieved in the sixth iteration, successfully resolved severe training instability by implementing a learning rate decay schedule. This stable and optimized architecture served as the foundation for an ensemble of models, which produced the final, competition-winning result.

![Final Model Training Curves](ML6(90.9%)/loss_plot.png)

---

## Project Highlights

This project demonstrates a robust, iterative approach to model development. Key challenges were diagnosed and solved methodically:

-   **Problem 1: Severe Overfitting:** Addressed by implementing **Dropout** regularization and **Early Stopping** to prevent the model from memorizing the training data.
-   **Problem 2: Class Imbalance:** A poorly performing class was identified using a confusion matrix and corrected with targeted **Data Augmentation** and **Class Weighting**.
-   **Problem 3: Training Instability:** Erratic validation performance was stabilized by introducing a **Learning Rate Decay Schedule**, the most critical step for achieving convergence.
-   **Final Optimization:** An **Ensemble Method** (majority vote) was applied to the best model to maximize the final Kaggle score, boosting it to **90.9%**.

---

## Tech Stack

-   **Frameworks:** TensorFlow, Keras, Scikit-learn
-   **Libraries:** NumPy, Pandas, Matplotlib
-   **Environment:** Python 3, Google Colab with GPU Acceleration

---

## How to Run This Project

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/your-project-repo.git
cd your-project-repo
```

### 2. Set Up the Environment
Create a virtual environment and install the required packages.
```bash
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

### 3. Download the Data
The data for this project is from the [INSERT KAGGLE COMPETITION LINK HERE] competition. Please download the dataset and place the `train/` and `test/` folders inside a `data/` directory at the root of this project.

### 4. Train the Model
Execute the main training script to start training the final model architecture.
```bash
python src/train.py
```
