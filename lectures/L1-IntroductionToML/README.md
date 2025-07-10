# Lecture 1: Introduction

This directory contains notes, code examples, and resources for Lecture 1 of the Machine Learning course, focusing on the course structure, assessment methods, foundational algorithms, and key challenges in machine learning. The lecture introduces core concepts that form the basis for subsequent topics in the course.

## Table of Contents
1. [Course Overview](#course-overview)
2. [Course Structure](#course-structure)
3. [Assessment](#assessment)
4. [Learning Platform](#learning-platform)
5. [Machine Learning Algorithms](#machine-learning-algorithms)
6. [Machine Learning Challenges](#machine-learning-challenges)
7. [Generalization](#generalization)
8. [Instance-Based vs. Model-Based Learning](#instance-based-vs-model-based-learning)
9. [Batch vs. Online Learning](#batch-vs-online-learning)

## Course Overview
The course provides in-depth knowledge of advanced machine learning concepts and current research trends. It is a 15-credit course spanning approximately 9 weeks (March to April), with an expected workload of 20 hours per week (50% of full-time study).

- **Objectives**:
  - Acquire advanced knowledge in machine learning.
  - Understand current research trends.
- **Workload**:
  - 15 credits (~130 hours total).
  - 20 hours/week.

## Course Structure
The course includes 14 lectures, lab assignments, a course project, and seminars.

- **Lectures**: 14 sessions, each ~2 hours, covering theoretical and practical aspects.
- **Assignments and Projects**: Practical tasks and a significant project.
  - Code: [Assignments](Assignments/)
- **Seminars**:
  - Paper seminar: Discussion of research papers.
  - Topic seminar: Focused on specific machine learning topics.

## Assessment
The course has 3–4 examination components, contributing to the 15 credits.

- **Components**:
  - Assignments and Paper Presentations (5 credits): Pass (G) or Fail (U).
  - Project (5 credits): Pass (G) or Fail (U).
  - Written Exam (5 credits): Graded from Excellent (A) to Fail (U), determines final grade.
- **Process**:
  - Submit reports by supervisor-set deadlines.
  - Receive feedback ("Ok" or "Complement") and revise if needed.
  - Approved reports lead to an oral examination; failed exams can be retaken.

## Learning Platform
The course uses the Canvas platform for:
- Posting course information.
- Uploading lecture slides.
- Submitting reports.
- Other course-related activities.

Code examples for Canvas integration: [Platform](Platform/)

## Machine Learning Algorithms
This section covers foundational algorithms introduced in the lecture.

### Logistic Regression
Used for binary classification (e.g., yes/no) using the sigmoid function to compute probabilities.

- Code: [LogisticRegression](LogisticRegression/logistic_regression.py)
- Example: Predicting pass/fail outcomes based on input features.

### Naive Bayes
Calculates the probability of a sample belonging to a category, assuming feature independence.

- Code: [NaiveBayes](NaiveBayes/naive_bayes.py)
- Example: Classifying text as positive or negative sentiment.

### K-Nearest Neighbors (KNN)
Classifies based on the k closest training samples (e.g., K=1).

- Code: [KNN](KNN/knn.py)
- Example: Classifying iris flowers based on feature similarity.

### Decision Trees
Represents decisions as a tree structure, akin to if-else statements.

- Code: [DecisionTrees](DecisionTrees/decision_tree.py)
- Example: Predicting customer churn based on decision rules.

## Machine Learning Challenges
Key challenges in machine learning include:

- **Data Issues**:
  - Insufficient data: Not enough data to train effectively.
  - Poor quality data: Noisy or incomplete data.
  - Irrelevant features: Features that do not improve performance.
- **Solutions**:
  - Ignore problematic attributes (e.g., missing age data).
  - Impute missing data (e.g., median values).
  - Feature selection, extraction, and engineering.

Code and experiments: [DataChallenges](DataChallenges/)

## Generalization
Generalization is a model's ability to perform well on unseen data.

- **Issues**:
  - Underfitting: Model is too simple, poor accuracy on training and test data.
  - Overfitting: Model fits training data too well, poor test accuracy.
- **Solutions**:
  - Use simpler models.
  - Increase training data.
  - Clean data to remove errors or outliers.

Code and experiments: [Generalization](Generalization/)

## Instance-Based vs. Model-Based Learning
- **Instance-Based**: Uses the entire dataset for predictions, high classification cost.
  - Example: KNN.
- **Model-Based**: Builds a model (e.g., linear function) for efficient predictions.
  - Example: Logistic Regression.

Code and experiments: [LearningTypes](LearningTypes/)

## Batch vs. Online Learning
- **Batch Learning**: Trains on the entire dataset, then deploys without further learning.
  - Example: Full-batch or mini-batch gradient descent.
- **Online Learning**: Learns incrementally as data arrives, suitable for continuous streams.
  - Requires tuning the learning rate.

Code and experiments: [BatchOnline](BatchOnline/)

## Getting Started
To run the code examples:
1. Clone the repository: `git clone https://github.com/[YourGitHubUsername]/ML-Course-Notes.git`
2. Navigate to the `Introduction` directory: `cd Introduction`
3. Install dependencies: `pip install -r requirements.txt`
4. Run specific scripts (e.g., `python LogisticRegression/logistic_regression.py`)

## Directory Structure

Introduction/

├── Assignments/

├── BatchOnline/

├── DataChallenges/

├── DecisionTrees/

│ └── decision_tree.py

├── Generalization/

├── KNN/

│ └── knn.py

├── LearningTypes/

├── LogisticRegression/

│ └── logistic_regression.py

├── NaiveBayes/

│ └── naive_bayes.py

├── Platform/

└── README.md


## Requirements
- Python 3.x
- Libraries: `scikit-learn`, `numpy`, `pandas` (see `requirements.txt`)

## Contributing
Contributions are welcome! Submit pull requests with additional notes, code, or corrections. Ensure code is documented and compatible with Python 3.x.

## License
This repository is licensed under the MIT License. See [LICENSE](../LICENSE) for details.
