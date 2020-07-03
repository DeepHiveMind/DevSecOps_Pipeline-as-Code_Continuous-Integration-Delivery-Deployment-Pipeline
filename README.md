# DevSecOps_Pipeline-as-Code_Continuous-Integration-Delivery-Deployment-Pipeline
This repo details out nunaces of following aspects with relevant codesets:
- DevSecOps | Pipeline-as-Code | 
- Continuous-Integration --> Continuous-Delivery ---> Continuous- Deployment 
- Overview of A Fully Automated DevSecOps CI CD Pipeline
- Automated DevSecOps CI CD Pipeline hosted at AWS (DevSecOps CI/CD Pipeline using Jenkins Multi-branch Pipelines hosted **at AWS** with **codeset**)
- DevOps CD Pipeline for AI/ML hosted at Azure (**DevOps in ML** -MLOPS Continuous Deployment flow **at Azure** based on DOCKER, KUBERNETES, HELM, KUBEFLOW, TESNORFLOW, TF-SERVING  with **codeset**)


# A Quick Rundown
- [CI Integration vs CD Delivery vs CD Deployment](#CI-Integration-vs-CD-Delivery-vs-CD-Deployment)
- [A Fully Automated DevSecOps CI CD Pipeline Overeview](#a-fully-automated-devsecops-ci-cd-pipeline-Overview)
- [Automated DevSecOps CI CD Pipeline hosted at AWS](#automated-devsecops-CI-CD-Pipeline-hosted-at-AWS)


# CI Integration vs CD Delivery vs CD Deployment

* CI == continuous integration, 
    - a practice that focuses on making preparing a release easier. 
    
* CD == either Continuous DELIVERY or Continuous DEPLOYMENT, 
     - while those two practices have a lot in common, they also have a significant difference that can have critical consequences for a business.
     
#### Vantage View of Broader Canvass 

Automated & Manual Steps coverage under Continuous Integration, Continuous Development & Continuous Deployment:
<br>
<img src="/assets/CICDCD.png" height="400" width="800" />
     
#### Continuous Integration Vs Continuous Development Vs Continuous Deployment


# A Fully Automated DevSecOps CI CD Pipeline Overview

#### Client's Ask 
Client is one of the largest business conglomerates in, with business verticals including telecom, retail, petrochemicals among others. They are on their digital transformation journey by embracing Cloud Computing, Agile and DevOps. Alongside, they also focused on **“shift left”** policy and **DevSecOps** for integrating security into their processes.

#### Goal
During the discussion with Client's VP-DevOps, requirements are zeroed in for the following goals:

- Integration of Jira with various Tools used in their entire product development life cycle
- Remove Manual Build and Deploy Process
- Embed security into their DevOps pipeline
- Implement efficient, continuous, automated and secure development and deployment process

#### SOLUTION
By using best practices of DevSecOps, an end to end secure continuous integration and continuous deployment pipeline is laid out for our customer.  took the following steps to achieve our goals:

- 1. Implement DevSecOps in Product Development Lifecycle
- 2. Implement Continuous Integration and Continuous Deployment (CI/CD) pipeline with Jenkins (CI Engine)
<br>
- 3. Integrate Jira (Agile Board) with GitHub (SCM)
- 4. Integrate Jira with Jenkins (CI Engine - Jenkins as a Code/Pipeline as a Code (JaaC/PaaC))
- 5. Integrate Jira with Confluence (Wiki)
- 6. Integrate Jira with Sonarqube (SCAT)
<br>
- 7. Configure Jenkins for Maven, Wheel & other code build tools (CBT)
- 8. Integrate Jenkins with Sonarqube (SCAT)
- 9. Integrate Jenkins with Nexus (Artefact Repository Manager)
- 10. Integrate Jenkins with Docker (Containers/Virtualization - Docker/RKT)
- 11. Integrate Jenkins with CLAIR (Container Vulnerability Scanner | Conatiner driven Common Vulnerability Scoring System CVSS)
- 12. Integrate Jenkins with Azure/ AWS (Cloud Service Provider - CSP)
- 13. Integrate Jenkins with Terraform/ AWS CloudFormation / AZURE Resource Manager / GCP Deployment Manager (IaC Tools)
<br>
- 14. Configure Jenkins for Ansible (Configuration Management tool for Multiple Environments)
- 15. Integrate Jenkins with K8S (openShift K8S/ AWS EKS/ AZURE AKS / GCP GKE/ Rancher)
- 16. Implement Build notification on emails and slack
<br>
- 17. Implement SIEM Monitoring Tool in Prod
- 18. Implement System Telemetry Tool in Prod
- 19. Implement Metering Tool in Prod

#### TECH STACK IN AZURE



# Automated DevSecOps CI CD Pipeline hosted at AWS

Refer to my other repo for [Automated DevSecOps CI CD Pipeline hosted at AWS](https://github.com/DeepHiveMind/Automated-DevSecOps-CI-CD-Pipeline-hosted-at-AWS).
    
Please note- 
    - The Above Repo is a private repo. Reach me on my contact details on https://DeepHiveMind.io for to get access for the same.
    

# DevOps CD Pipeline for AI ML hosted at Azure

Refer to my following other Repo for the deep dive.
- [DevOps in ML MLOPS Flow based on DOCKER KUBERNETES HELM KUBEFLOW](#MLOPS-Architecture-based-on-KUBEFLOW)

     - [Train and Serve TensorFlow Models at Scale with KUBERNETES and KUBEFLOW](#Train-and-Serve-TensorFlow-Models-at-Scale-with-Kubernetes-and-Kubeflow)
			
		- [DOCKER - Containerizatioin of AI Modules](https://github.com/DeepHiveMind/Kubeflow-AI-Labs/tree/master/1-docker)
		- [KUBERNETES - K8S for AI](https://github.com/DeepHiveMind/Kubeflow-AI-Labs/tree/master/2-kubernetes)
		- [HELM Charts on K8S for AI complex deployment](https://github.com/DeepHiveMind/Kubeflow-AI-Labs/tree/master/3-helm)
		- [KUBEFLOW for AI MLOPS](https://github.com/DeepHiveMind/Kubeflow-AI-Labs/tree/master/4-kubeflow)
		- [JupyterHub on K8S- AI Build Notebook](https://github.com/DeepHiveMind/Kubeflow-AI-Labs/tree/master/5-jupyterhub)
		- [TFJob- K8S custom kind for AI Training on GPU/CPU/TPU](https://github.com/DeepHiveMind/Kubeflow-AI-Labs/tree/master/6-tfjob) 
		- [Distributed Tensorflow](https://github.com/DeepHiveMind/Kubeflow-AI-Labs/tree/master/7-distributed-tensorflow)
		- [Hyperparameters Sweep with Helm](https://github.com/DeepHiveMind/Kubeflow-AI-Labs/tree/master/8-hyperparam-sweep)
		- [AI Model Serving for prediction/scoring](https://github.com/DeepHiveMind/Kubeflow-AI-Labs/tree/master/9-serving)

Interested in full view of **Enterprise AI MLOPS**. Refer to my repo dedicated to **[EnterpriseAI_Platform_MLOps](https://github.com/DeepHiveMind/EnterpriseAI_Platform_MLOps)** with great depth insight into MLOPS.
