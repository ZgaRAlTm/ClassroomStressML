Classroom Stress Detection using Wearable Sensors and Machine Learning
Overview
This repository contains the code and resources for a proof-of-concept study exploring stress detection in educational settings using wearable sensors and machine learning techniques. The research spans 18 weeks and involves collecting biometric data from five undergraduates during classroom sessions using Hexoskin vests and Actigraph watches.
Key Features
* Data collection using Hexoskin vests and Actigraph watches
* Analysis of heart rate, respiration rate, breathing volume, and movement data
* Application of machine learning algorithms (Random Forest, K-Nearest Neighbors, XGBoost, Neural Networks)
* Exploration of temporal dynamics in stress detection
* Comparison of generalized models, leave-one-subject-out (LOSO) models, and person-specific models (PSM)
Repository Contents
1. ACTI-HEXO-VIS.ipynb: Jupyter notebook for visualizations combining Actigraph and Hexoskin data
2. All Models and Graphs.ipynb: Comprehensive notebook containing all models and graphical representations
3. HEXO_ONLY_VIS.ipynb: Visualizations focused on Hexoskin data
4. Unsupervised Learning -- PCA.ipynb: Principal Component Analysis for feature exploration
Dependencies
Ensure you have the following Python libraries installed:
Copy
numpy==1.21.5
pandas==1.3.5
matplotlib==3.5.1
seaborn==0.11.2
scikit-learn==1.0.2
xgboost==1.5.2
scipy==1.7.3
plotly==5.6.0
You can install these dependencies using pip:
Copy
pip install -r requirements.txt
Getting Started
To replicate the study or explore the data:
1. Clone this repository:
Copy
git clone https://github.com/YourUsername/ClassroomStressML.git

2. Install the required dependencies:
Copy
pip install -r requirements.txt

3. Data Preprocessing:
   * Ensure you have the raw data from Hexoskin vests and Actigraph watches
   * Use the data cleaning and preprocessing methods described in the research paper
   * Save the preprocessed data in a format compatible with the analysis notebooks
   4. Analysis: You can run any of the following Jupyter notebooks independently for their respective portions of the analysis:
   * HEXO_ONLY_VIS.ipynb: For initial Hexoskin data visualization
   * ACTI-HEXO-VIS.ipynb: For combined Actigraph and Hexoskin data visualization
   * Unsupervised Learning -- PCA.ipynb: For feature exploration using Principal Component Analysis
   * All Models and Graphs.ipynb: For comprehensive model training and evaluation
   5. Each notebook is self-contained and can be run separately to focus on specific aspects of the analysis. However, for a complete understanding of the project, it's recommended to go through all notebooks.
Key Findings
   * Random Forest model achieved the highest accuracy (median F1 score of 92%)
   * Breathing volume emerged as the most significant predictor of stress
   * Individualized models consistently outperformed generalized ones
   * A 30-day sliding window was found optimal for stress classification
Methodology
   1. Data Collection: Utilized Hexoskin vests and Actigraph watches to collect physiological data from participants during classroom sessions.
   2. Data Preprocessing: Cleaned and processed raw sensor data, handling missing values and outliers.
   3. Feature Engineering: Extracted relevant features from the preprocessed data.
   4. Exploratory Data Analysis: Visualized data distributions and relationships using various plots and statistical techniques.
   5. Model Development: Implemented and compared multiple machine learning models, including Random Forest, K-Nearest Neighbors, XGBoost, and Neural Networks.
   6. Model Evaluation: Assessed model performance using metrics such as accuracy and F1 score, employing cross-validation techniques.
   7. Temporal Analysis: Explored the temporal dynamics of stress using sliding window approaches.
Future Work
   * Expand the study to include larger and more diverse samples
   * Explore applications in various high-stress environments
   * Develop real-time stress detection and intervention systems
   * Investigate the integration of additional physiological sensors
   * Implement more advanced deep learning techniques for improved accuracy
Contributors
   * Latherial Calbert, Department of Mathematics, College of Charleston
   * Navid Hashemi Tonekaboni, Department of Computer Science, College of Charleston
Acknowledgments
We thank the College of Charleston's Data Mining and Connectivity (DMC) Research Lab for providing essential equipment. OpenAI's ChatGPT was used for grammar and syntax refinement in the research paper.
Citation
If you use this code or findings in your research, please cite our paper:
Copy
Calbert, L., & Tonekaboni, N. H. (2024). Temporal Dynamics of Classroom Stress: Insights from Wearable Sensors and Machine Learning.