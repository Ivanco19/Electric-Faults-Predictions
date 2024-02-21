# Electrical Fault Prediction

### Overview
Electrical faults can have critical implications for power systems, leading to downtime, damage, and safety risks. In this project, we leverage machine learning techniques, specifically Support Vector Machines (SVM), Random Forest (RF), Decision Trees (DT), and K-Nearest Neighbors (KNN), to predict and prevent electrical faults. 

Electrical systems are susceptible to various types of faults, which can be broadly classified into symmetric and asymmetric faults. Understanding these classifications is crucial for effective fault detection and prevention in power systems. Typical relative frequencies of occurrence of different kinds of faults in a power system are:

1. Symetric Faults:
    * Three phase (LLL) - Less than 5%
    * Three phase to Ground (LLL-G) - Less than 5%

2. Asymmetric Faults:
    * Line to Ground (L-G) - 70%
    * Line to Line (L-L) - 15%
    * Double Line to Ground (LL-G) - 10%

What happens during a fault?

During a fault, both current and voltage undergo alterations. For instance, in a line-to-ground fault, current flows towards the ground, causing a reduction in voltage. In the case of bifasic faults, a short circuit occurs between two lines, resulting in significant fluctuations in both current and voltage. These abrupt changes serve as the distinctive signature for each type of fault. 

### Project Process
1. Data Preprocessing: Before diving into modeling, we preprocess the dataset to ensure its suitability for machine learning algorithms. This involves tasks such as handling missing values, adding or dropping columns, etc.

2. Data Visualization: Exploratory Data Analysis (EDA) and visualization techniques are employed to gain insights into the dataset. Visualization aids in understanding patterns, correlations, and potential challenges in the data.

3. Data Modeling: This stage involves creating machine learning models using SVM, RF, DT, and KNN algorithms. Techniques such as label encoding and standard scaling are applied to prepare the data for training.

4. Data Evaluation: The models are evaluated using key metrics such as accuracy, precision, and recall. The process involves a meticulous analysis of each model's performance to identify strengths and weaknesses.

### Project Scenarios
* Scenario 1: Original Dataset
In the first scenario, the models were trained and tested on the original dataset. While achieving satisfactory accuracies (around 90% for all models), challenges arose in distinguishing between LLL and LLL-G faults.

* Scenario 2: Combined Fault Types
Recognizing the difficulties in Scenario 1, we combined LLL and LLL-G faults into a single category in the second scenario. This modification resulted in significantly improved results, with accuracies, precision, and recall reaching approximately 99%.

### Cross-Validation
Each algorithm underwent five fold cross-validation to ensure robust and reliable model performance.

### Conclusion
This project emphasizes the significance of predicting electrical faults and showcases the impact of preprocessing, visualization, modeling, and evaluation in enhancing the effectiveness of machine learning models.
