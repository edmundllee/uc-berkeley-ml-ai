### Can voice-based biomedical features be used to predict Parkinson's disease?

**Author**
Edmund Lee

#### Executive summary
Parkinson's Disease (PD), a nervous system disorder that gets progressively worst over time, lacks a definitive test and early clinical diagnosis. Being subjective, the clinical test could lead to misdiagnosis (confusing PD with Multiple System Atrophy (MSA), Progressive Supranuclear Palsy (PSP), and/or Corticobasal Degeneration (CBD)). Even the DATScan, perhaps the most used tool, cannot distinguish between them and while MRI analyzed with AI can reach high accuracy, it's expensive and not yet be widely available.

Enter Speech. 90% of individuals with Parkinson's develop a characteristic set of speech impairments known as hypokinetic dysarthria. Can we use voice-based biomarkers to contribute to the prediction of Parkinson's Disease?


#### Rationale
Why should anyone care about this question?
While there has been recent advancement in discovering biomarkers for Parkinson's, many patients still rely on clinical based evidence to diagnose the disease. Parkinson's disease greatly impacts speech/motor function and being able to test this remotely in a scalable manner could have great impact in patient care with early diagnosis.

#### Research Question
What are you trying to answer?
Identify machine learning models capable of predicting motor_UPDRS values from voice-derived features highlighting features predicting Parkinson.

#### Data Sources
What data will you use to answer you question?
Parkinson's Telemonitoring dataset: publicly available from the UCI Machine Learning Repository

#### Methodology
What methods are you using to answer the question?
* Exploratory Data Analysis (EDA)
* Principal Component Analysis (PCA)
* Linear Regression
* Decision Trees
* Support Vector Machines (SVM)

#### Results
What did your research find?
* Jitter(%), Shimmer, and NHR increased in value across UPDRS severity quartiles.

* Baseline Model (Linear Regression) Results: (RMSE): ~7.51, R² Score: ~0.12 

* Top features were Jitter(Abs), Jitter:RAP, Shimmer:APQ3, Jitter:DDP, and Shimmer:DDA

#### Next steps
What suggestions do you have for next steps?
* Try other models 
* Exposed as API
* Create a private, offline-first, multimodal model application
    * speech: use exposed API
    * video: analyze gait (walking patterns)
    * face: smile (and facial expression)
    * text: spiral test
    * image: DATScan, MRI, handwriting (micrographia)
 


#### Outline of project

- [Link to module 20.1](https://github.com/edmundllee/uc-berkeley-ml-ai/blob/main/module-20/notebooks/parkinson_prediction.ipynb)

##### Contact and Further Information
edmundlee@yahoo.com