Quick Links: [Official Paper](https://www.computer.org/csdl/proceedings-article/hiset/2024/607000a128/21MMhRlfai4) | [Dataset Used](https://archive.ics.uci.edu/dataset/45/heart+disease) | [Metadata](https://github.com/uci-ml-repo/ucimlrepo) | [Project Setup](#project-setup) | [Run Project](#4-run-project)

# Heart Disease Prediction using 
## 1. Objective of the Paper:

The main purpose of this paper is to explore the potential of data mining and machine learning algorithms in predicting Coronary Artery Disease (CAD). It aims to review existing research on CAD prediction using these techniques and to advocate for their use in early detection to reduce mortality and healthcare costs. The paper emphasizes the importance of effectively utilizing the vast amounts of healthcare data for improved disease prediction and patient care.

## 2. Motivation for the Study:

- **Rising Prevalence of CAD**: CAD is a leading cause of death worldwide, particularly in developing nations.

- **Challenges in Traditional Diagnosis**: Traditional methods for CAD detection can be expensive, require expertise, and may not be efficient for large-scale patient checks.

- **Underutilized Healthcare Data**: Healthcare systems generate massive amounts of data that are often not effectively used for predictive insights.

- **Potential of Data Mining and Machine Learning**: These techniques offer the potential to extract valuable information from patient data to identify patterns and predict diseases like CAD in early stages, potentially saving lives and reducing healthcare expenses.

## 3. Dataset Used (in Reviewed Studies):

The paper frequently mentions the UCI Machine Learning Repository, specifically the Cleveland heart disease dataset. This dataset is described as having:

- 303 instances (records) in some studies, and 401 records in another study mentioned in the literature review.

- 76 attributes/characteristics originally, but many studies reviewed focused on using a reduced set of 14 or 17 key features/characteristics for prediction.

## 4. Algorithms Used (in Reviewed Studies):

The literature review section highlights various data mining and machine learning algorithms used in previous studies for CAD prediction. These include:

### Classification Algorithms:

- **Decision Trees**: J48, ID3, CART (Classification and Regression Tree), Logistic Model Tree  
- **Naive Bayes** (including Hybrid Genetic Naive Bayes)
- **K-Nearest Neighbors (KNN)**
- **Support Vector Machines (SVM)** (mentioned in the concluding summary of literature review, though not detailed in individual study descriptions)
- **Artificial Neural Networks (ANNs)**: Multilayer Perceptron with Backpropagation
- **Fuzzy Rule-Based Systems**

### Other Techniques:
- **Association Rule Mining** (used in conjunction with classification)
- **Genetic Algorithms** (for feature selection and model optimization)
- **Ensemble Methods**: Bagging, Boosting, Random Forest (mentioned in the concluding summary of literature review)
- **Clustering Algorithms**: Modified K-Means (mentioned in one study)

### Tools Used:
- **WEKA**: Frequently mentioned as a tool for experimentation and implementation in several reviewed studies.
- **MATLAB**: Used in one study for implementing a neural network model.
- **Hadoop**: Mentioned in one study for big data analytics in healthcare.

## 5. Key Findings and Discussions (from Literature Review and Discussions Section):
- **Data Mining and Machine Learning are Effective**: The reviewed literature suggests that data mining and machine learning techniques have been successfully applied to CAD prediction and show promising results.
- **Hybrid Models Show Promise**: Several studies explored hybrid models (combinations of multiple algorithms) and found that they often achieve higher accuracy and precision compared to single models. Combining different techniques can leverage the strengths of each method.
- **Feature Selection is Important**: Many studies focused on selecting relevant features from the dataset to improve model performance and reduce complexity.
- **Different Algorithms have Varying Performance**: The accuracy and effectiveness of different algorithms vary. Some studies found J48 to be more accurate than Relational Model Tree, while others highlighted the effectiveness of Naive Bayes or hybrid approaches.
- **Importance of Data Quality**: The conclusion emphasizes that the accuracy of machine learning algorithms depends on the quality of the training dataset.
- **Tools like WEKA and MATLAB are Useful**: These tools are valuable for data analysis, model building, and experimentation in the medical domain.

## 6. Conclusions of the Paper:
- **Potential of Data Mining and Machine Learning in Healthcare**: The paper concludes that data mining and machine learning have significant potential in healthcare, particularly for disease detection and prediction. They can offer cost-effective and efficient alternatives to traditional diagnostic methods.
- **Early Detection is Crucial**: Early detection of CAD is vital for reducing mortality and improving patient outcomes. Machine learning can contribute to this by identifying individuals at risk in earlier stages.
- **Future Directions**:
    - **Focus on Data Cleaning and Preprocessing**: The paper suggests future work should focus on improving data cleaning and preprocessing methods to create better datasets for mining.

    - **Explore More Machine Learning Algorithms**: Further research should explore and apply a wider range of machine learning algorithms for CAD prediction.

    - **Reduce Mortality from CAD**: The ultimate goal is to use these techniques to reduce the number of deaths caused by CAD.

In summary, this paper provides a literature review highlighting the application of data mining and machine learning for Coronary Artery Disease prediction. It emphasizes the potential of these techniques, particularly hybrid approaches, to improve early detection, reduce healthcare costs, and ultimately decrease mortality associated with CAD. The paper advocates for continued research in this area, focusing on data quality and exploring a broader range of algorithms to refine prediction models.
<br>
<br>
<br>
# Project Setup

NOTE: If you don't want to use uv, you can use pip to install the dependencies. But I highly recommend using uv as it is much better than pip. You need to replace `uv run` with `python` in the commands below.

## 1. Install UV - Python Package Manager (better than pip)

- #### For Mac/Linux
    ```bash
    curl -LsSf https://astral.sh/uv/install.sh | sh
    ```

- #### For Windows
    ```PowerShell
    powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
    ```

- To update uv: `uv self update`

## 2. Clone Project
```bash
https://github.com/lkx100/heart-disease-prediction.git
cd heart-disease-prediction
```

## 3. Install dependencies
```bash
uv sync
```

## 4. Run project
```bash
uv run manage.py runserver
```  

***

If you need a full guide on how to install uv, you can read my blog [here](https://acecoderbeta.onrender.com/blogpost/post/best-python-package-manager-uv/) or check out for the [official documentation](https://docs.astral.sh/uv/).
