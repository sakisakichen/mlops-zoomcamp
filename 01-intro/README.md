Notes from [balapriyac](https://github.com/balapriyac/DTC-MLOps-Zoomcamp/blob/main/week1/intro_setup.md)

## MLOps Intro 

When you are designing a machine learning system, your job doesn't end with building the model—and achieving a high accuracy score and a low validation error! For the model to be actually helpful—you will have to consider deploying it, and also ensure that the model's performance does not degrade over time. And MLOps is a set of *best practices* for putting machine learning models into production.

![image](https://user-images.githubusercontent.com/47279635/168582280-52820583-d0bb-4b46-add4-b2fa4c09bc1b.png)

###  Steps in a Machine Learning Project
The various stages in a machine learning project can be broadly captured in the following three steps:
1. **Design**: In the `design` step, you are considering the problem at hand—to decide whether or not you'll need a machine learning algorithm to achieve the objective. 
2. **Train**: Once you decide on using a machine learning algorithm, you `train` the model and optimize its performance on the validation dataset.
3. **Operate**: The `operate` state captures the performance of the model after it's deployed. Some of the questions that you'll answer throughout the course, include:
  - If the performance of the model degrades, can you retrain the model in a cost-effective manner?
  - How do you ensure that the deployed model performs as expected—that is, how do you monitor the model's performance in production?
  - What are the challenges associated with monitoring ML models?

## MLOps Environment Setup

[GitHub Codespaces](https://www.youtube.com/watch?v=MzcmWXYxi2s&list=PL3MmuxUbc_hIUISrluw_A7wDSmfOhErJK&index=3)


## MLOps Maturity Model
notes from [LoHertel](https://github.com/LoHertel) 

| Lvl |              | Overview | Use Case | 
|----:|--------------|----------|----------|  
| 0️⃣  | **No MLOps** | <ul><li>ML process highly manual</li><li>poor cooperation</li><li>lack of standards, success depends on an individual's expertise</li> </ul> | <ul><li>proof of concept (PoC)</li><li>academic project</li></ul> |
| 1️⃣  | **DevOps but no MLOps** | <ul><li>ML training is most often manual </li><li>software engineers might help with the deployment</li><li>automated tests and releases</li> </ul> | <ul><li>bringing PoC to production</li></ul> |
| 2️⃣  | **Automated Training** | <ul><li>ML experiment results are centrally tracked </li><li>training code and models are version controlled</li><li>deployment is handled by software engineers</li> </ul> | <ul><li>maintaining 2-3+ ML models</li></ul> |
| 3️⃣  | **Automated Model Deployment** | <ul><li>releases are managed by an automated CI/CD pipeline</li><li>close cooperation between data and software engineers</li><li>performance of the deployed model is monitored, A/B tests for model selection are used</li></ul> | <ul><li>business-critical ML services</li></ul> |
| 4️⃣  | **Full MLOps Automated Operations** | <ul><li>clearly defined metrics for model monitoring</li><li>automatic retraining triggered when passing a model metric's threshold</li> </ul>  | <ul><li>use only when a favorable trade-off between implementation cost and increase in efficiency is likely</li><li>retraining is needed often and is repetitive (has potential for automation)</li></ul> |


A high maturity level is not always needed because it comes with additional costs.   
The trade-off between automated model maintenance and the required effort to set up the automation should be considered.   
An ideal maturity level could be picked based on the use case / SLAs and the number of models deployed.  
