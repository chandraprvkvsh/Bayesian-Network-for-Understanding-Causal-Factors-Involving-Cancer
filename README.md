# Brief Introduction

Objective of this project was to build a Probabilistic Graphical Model and learning the cause and effect relationship between factors affecting cancer and making queries on the model,

Query 1: Will the patient be having ‘tuberculosis’ given that the patient smokes but no problem of dyspnoea?
Query 2: What is the most probable value of ‘x ray’ conditioning patient is from asia and has lung cancer?
Query 3: What is the most probable value of bronc if patient has the issue of dyspnoea , he is from asia but does not have either of the diseases?

The project involved building the model, Using MLE to generate CPD for all the nodes present in model and using Variable Elimination algorithm for solving  Query1, Query2 and Query3.

Bayesian model, Variable elimination, Maximum likelihood estimator from PGMPY were used.

# Details of the project

The Cancer data set contains the following variables:

D (dyspnoea), a two-level factor with levels yes and no
T (tuberculosis), a two-level factor with levels yes and no
L (lung cancer), a two-level factor with levels yes and no
B (bronchitis), a two-level factor with levels yes and no
A (visit to Asia), a two-level factor with levels yes and no
S (smoking), a two-level factor with levels yes and no
X (chest X-ray), a two-level factor with levels yes and no
E (tuberculosis versus lung cancer/bronchitis), a two-level factor with levels yes and no

Fit the following Bayesian Model to the above dataset using maximum likelihood estimator and perform the inference for the following queries:

Query1: Will the patient be having ‘tuberculosis’ given that the patient smokes but no problem of dyspnoea?

Query2: What is the most probable value of ‘xray’ conditioning patient is from asia and has lung cancer?

Query 3: What is the most probable value of bronc if patient has the issue of dyspnoea , he is from asia but does not have either of the diseases?

Carry out the following tasks:

1. Load and read the data from "Data.csv"
2. Create a Bayesian Model as shown in figure
3. Using MLE, generate CPD for all the nodes present in model
4. Using Varibable Elimination algorithm, solve Query1, Query2 and Query3, as per the evidences mentioned in queries (Yes=1 and No=0)
5. Write the output to "output.csv"
