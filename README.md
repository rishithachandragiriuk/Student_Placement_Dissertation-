# Student_Placement_Dissertation-

# Author Name : Chandragiri Rishitha

# Student id : 35040415

## 1. Project Overview

This project develops and evaluates a student placement prediction framework using Machine Learning (ML) and Deep Learning (DL) approaches. The framework uses academic, technical, training and employability-related student attributes to predict placement outcomes.

The complete workflow covers data preprocessing, class balancing using Synthetic Minority Over-sampling Technique (SMOTE), baseline model development, hyperparameter optimisation, systematic model evaluation, SHAP analysis, prototype development and human evaluation.

The final selected model is Logistic Regression.

## 2. Dissertation Aim

The main aim is to develop and evaluate an optimised Machine Learning and Deep Learning framework for student placement prediction, supported by SHAP analysis, prototype development and human evaluation.

## 3. Research Question

How effectively can an optimised Machine Learning and Deep Learning framework predict student placement outcomes through hyperparameter tuning, SHAP, prototype development and human evaluation?

## 4. Objectives

1. Analyse and preprocess student academic, technical and employability-related data.
2. Develop and evaluate selected Machine Learning and Deep Learning models for student placement prediction.
3. Optimise model performance through systematic hyperparameter tuning and evaluate the resulting models using appropriate performance metrics, with F1-score as the primary metric.
4. Apply SHAP to identify and analyse the key student-related features influencing placement predictions.
5. Develop and evaluate a GUI-based prototype using the best-performing model and assess its usability and usefulness through human feedback.

## 5. Dataset

The project uses the publicly available Kaggle Placement Prediction Dataset.

The dataset contains approximately 10,000 student records and includes student-level academic, technical, training and employability-related attributes.

Important variables include:

- StudentID
- CGPA
- Internships
- Projects
- Workshops/Certifications
- SoftSkillsRating
- PlacementTraining
- HSC_Marks
- SSC_Marks
- AptitudeTestScore
- ExtracurricularActivities
- PlacementStatus

The target variable is the student placement status, making the task a binary classification problem.

## 6. Methodology

The implemented workflow follows these main stages:

1. Dataset acquisition
2. Data inspection
3. Data preprocessing
4. Feature preparation
5. Feature scaling
6. Train-test splitting
7. Class balancing using SMOTE
8. Baseline model development
9. Hyperparameter optimisation
10. Tuned model evaluation
11. Best model selection using F1-score
12. SHAP analysis
13. GUI prototype development
14. Human evaluation design
15. Results and discussion

## 7. Models

Four predictive models were evaluated:

### Logistic Regression

Logistic Regression was used as a supervised classification model for predicting placed and non-placed students.

### Random Forest

Random Forest was included as an ensemble tree-based model capable of modelling nonlinear relationships.

### Support Vector Machine

Support Vector Machine was used to identify a suitable decision boundary between the placement classes.

### Artificial Neural Network

Artificial Neural Network was included as the Deep Learning approach for modelling nonlinear relationships between student attributes and placement outcomes.

## 8. Evaluation Metrics

The following evaluation metrics were used:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC

F1-score was treated as the primary metric because it provides a balance between precision and recall.

## 9. Hyperparameter Optimisation

GridSearchCV with five-fold cross-validation was used for systematic hyperparameter optimisation.

The purpose was to identify suitable model parameter combinations and determine whether optimisation could improve predictive performance.

## 10. Baseline Results

### Logistic Regression

Accuracy: 79.30%

Precision: 72.21%

Recall: 81.28%

F1-score: 76.48%

ROC-AUC: 87.64%

### Random Forest

Accuracy: 78.60%

Precision: 73.53%

Recall: 75.48%

F1-score: 74.49%

ROC-AUC: 86.73%

### Support Vector Machine

Accuracy: 79.05%

Precision: 72.40%

Recall: 79.83%

F1-score: 75.93%

ROC-AUC: 86.62%

### Artificial Neural Network

Accuracy: 79.30%

Precision: 76.14%

Recall: 72.83%

F1-score: 74.44%

ROC-AUC: 87.39%

## 11. Tuned Model Results

### Logistic Regression

Accuracy: 79.30%

Precision: 72.21%

Recall: 81.28%

F1-score: 76.48%

ROC-AUC: 87.64%

Cross-validation accuracy: 79.83%

### Random Forest

Cross-validation accuracy: 82.01%

Testing accuracy: 79.25%

Precision: 74.44%

Recall: 75.97%

F1-score: 75.19%

ROC-AUC: 87.10%

### Support Vector Machine

Cross-validation accuracy: 80.19%

Testing accuracy: 78.60%

Precision: 71.69%

Recall: 79.83%

F1-score: 75.54%

ROC-AUC: 83.40%

### Artificial Neural Network

Validation accuracy: 80.25%

Testing accuracy: 78.65%

Precision: 75.74%

Recall: 71.26%

F1-score: 73.43%

ROC-AUC: 87.28%

## 12. Best Performing Model

Logistic Regression was selected as the final model.

The final performance was:

Accuracy: 79.30%

Precision: 72.21%

Recall: 81.28%

F1-score: 76.48%

ROC-AUC: 87.64%

The main reason for selecting Logistic Regression was its strongest overall F1-score together with strong recall and ROC-AUC. The selection was therefore based on balanced performance rather than accuracy alone.

## 13. SHAP Analysis

SHAP was applied to the selected Logistic Regression model to identify influential student attributes.

The most influential features were:

1. AptitudeTestScore: approximately 0.51 mean absolute SHAP value
2. PlacementTraining: approximately 0.35
3. ExtracurricularActivities: approximately 0.32
4. SSC_Marks: approximately 0.26
5. SoftSkillsRating: approximately 0.26
6. HSC_Marks: approximately 0.26
7. CGPA: approximately 0.20
8. Projects: approximately 0.18
9. Workshops/Certifications: approximately 0.07

AptitudeTestScore was the strongest feature identified by the SHAP analysis.

The SHAP dependence analysis also indicated a positive relationship between AptitudeTestScore and its contribution to model output.

## 14. Prototype

A GUI-based Student Placement Prediction and Career Recommendation Prototype was developed.

The prototype allows student information to be entered through a graphical interface and provides a placement prediction using the selected model.

The interface includes fields for academic, training, technical and employability-related information.

The prototype contains controls for:

- Predict Placement
- Clear
- Exit
- Save Feedback
- Reset Evaluation

The prediction interface is integrated with the selected predictive model.

## 15. Human Evaluation

A human evaluation structure was developed to assess the practical usability and user experience of the prototype.

The evaluation template contains 200 participant records, identified from P001 to P200.

Five evaluation factors use a 1 to 5 rating scale.

The evaluation also includes:

- Overall rating
- Recommendation response
- Open feedback/comments
- Additional evaluation information

The evaluation is intended to assess usability, interface quality, prediction experience and overall acceptance.

Important note: the dissertation file contains the evaluation structure and participant records but does not contain completed numerical ratings. Therefore, numerical participant satisfaction averages should not be presented as completed results unless actual completed evaluation data are added.

## 16. Project Strengths

The main strengths of the project are:

- Structured preprocessing and modelling workflow
- Use of class balancing
- Evaluation of both ML and DL approaches
- Systematic hyperparameter optimisation
- F1-score-based model selection
- SHAP feature analysis
- Practical GUI prototype
- Human evaluation framework
- Integration of prediction and feature analysis

## 17. Project Limitations

The main limitations are:

1. The evaluation is based on one placement dataset.
2. External validation on independent institutional datasets was not performed.
3. The binary placement outcome does not represent job role, salary or employment sector.
4. Student populations may have different characteristics across institutions.
5. The human evaluation structure is available, but completed numerical participant ratings are not contained in the current dissertation file.
6. The prototype is a project-level implementation rather than a full institutional deployment.

## 18. Future Work

Future work can extend the project through:

1. Testing the framework on external placement datasets.
2. Using datasets from multiple educational institutions.
3. Incorporating longer-term employment outcomes.
4. Including job role, employment sector and salary information.
5. Expanding the human evaluation with completed participant responses.
6. Evaluating the prototype with a broader user population.
7. Investigating additional advanced ML and DL models.
8. Extending SHAP analysis to additional models and feature interactions.
9. Improving the prototype for wider practical use.
10. Conducting longer-term evaluation of prediction usefulness.

## 19. Key Results Summary

| Model | Accuracy | Precision | Recall | F1-score | ROC-AUC |
|---|---:|---:|---:|---:|---:|
| Logistic Regression | 79.30% | 72.21% | 81.28% | 76.48% | 87.64% |
| Random Forest | 78.60% | 73.53% | 75.48% | 74.49% | 86.73% |
| Support Vector Machine | 79.05% | 72.40% | 79.83% | 75.93% | 86.62% |
| Artificial Neural Network | 79.30% | 76.14% | 72.83% | 74.44% | 87.39% |

## 20. Key Numbers 
Dataset: approximately 10,000 student records

Number of models: 4

Primary metric: F1-score

Selected model: Logistic Regression

Accuracy: 79.30%

Precision: 72.21%

Recall: 81.28%

F1-score: 76.48%

ROC-AUC: 87.64%

GridSearchCV: 5-fold cross-validation

Top SHAP feature: AptitudeTestScore

Top SHAP value: approximately 0.51

Second important feature: PlacementTraining

PlacementTraining SHAP value: approximately 0.35

Third important feature: ExtracurricularActivities

ExtracurricularActivities SHAP value: approximately 0.32

Human evaluation records: 200

Participant identifiers: P001 to P200

Human evaluation scale: 1 to 5

## 23. Final Statement

The project demonstrates an integrated student placement prediction workflow that combines predictive modelling, optimisation, SHAP analysis, prototype development and human evaluation. Logistic Regression provided the strongest final testing performance according to the primary F1-score criterion, while SHAP analysis highlighted the student attributes most strongly associated with model predictions. The prototype provides a practical interface for applying the selected model to student placement prediction.
