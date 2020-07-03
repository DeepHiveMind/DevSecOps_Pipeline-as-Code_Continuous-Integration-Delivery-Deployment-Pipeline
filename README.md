# DevSecOps_Pipeline-as-Code_Continuous-Integration-Delivery-Deployment-Pipeline
This repo details out nunaces of following aspects with relevant codesets:
- DevSecOps | Pipeline-as-Code | 
- Continuous-Integration --> Continuous-Delivery ---> Continuous- Deployment 
- Overview of A Fully Automated DevSecOps CI CD Pipeline
- Automated DevSecOps CI CD Pipeline hosted at AWS (DevSecOps CI/CD Pipeline using Jenkins Multi-branch Pipelines hosted **at AWS** with **codeset**)
- DevOps CD Pipeline for AI/ML hosted at Azure (**DevOps in ML** -MLOPS Continuous Deployment flow **at Azure** based on DOCKER, KUBERNETES, HELM, KUBEFLOW, TESNORFLOW, TF-SERVING  with **codeset**)


# A Quick Rundown | Agenda
- [CI Integration vs CD Delivery vs CD Deployment](#CI-Integration-vs-CD-Delivery-vs-CD-Deployment)
- [A Fully Automated DevSecOps CI CD Pipeline Overeview](#a-fully-automated-devsecops-ci-cd-pipeline-Overview)
- [Automated DevSecOps CI CD Pipeline hosted at AWS](#automated-devsecops-CI-CD-Pipeline-hosted-at-AWS)
- [DevOps CD Pipeline for AI ML hosted at Azure](#DevOps-CD-Pipeline-for-AI-ML-hosted-at-Azure)


# CI Integration vs CD Delivery vs CD Deployment

***
* CI == continuous integration, 
    - a practice that focuses on making preparing a release easier. 
    
* CD == either Continuous DELIVERY or Continuous DEPLOYMENT, 
     - while those two practices have a lot in common, they also have a significant difference that can have critical consequences for a business.
 ***
 
 
#### Vantage View of Broader Canvass 

Automated & Manual Steps coverage under Continuous Integration, Continuous Development & Continuous Deployment:
<br>
<img src="/assets/CICDCD.png" height="400" width="800" />
     
#### Phases in a continuous Delivery pipeline

The architecture of the product that flows through the pipeline is a key factor that determines the anatomy of the continuous delivery pipeline. A highly coupled product architecture generates a complicated graphical pipeline pattern where various pipelines get entangled before eventually making it to production.

The product architecture also influences the different phases of the pipeline and what artifacts are produced in each phase. Let’s discuss the four common phases in continuous delivery:

 - CD Component phase:
 
*The pipeline first builds components - the smallest distributable and testable units of the product. For example, a library built by the pipeline can be termed a component. A component can be certified, among other things, by code reviews, unit tests, and static code analyzers.*
 	
	- Code reviews
	- Unit tests 
	- Static code analysis ...
	
- CD Sub-System phase:

*Loosely coupled components make up subsystems - the smallest deployable and runnable units. For example, a server is a subsystem. A microservice running in a container is also an example of a subsystem. 

As opposed to components, subsystems can be stood up and validated against customer use cases.*

  	- Functional tests
	- performance benchmarks
	- security vulnerabilities

- CD System phase:

*Once subsystems meet functional, performance, and security expectations, the pipeline could be taught to assemble a system from loosely coupled subsystems in cases where the entire system has to be released as a whole. What that means is that the fastest team can go at the speed of the slowest team. Reminds me of the old saying, “A chain is only as strong as its weakest link”.*

*System can be certified by integration, performance, and security tests. Unlike subsystem phase, do not use mocks or stubs during testing in this phase. Also, focus on testing interfaces and network more than anything else.*

*The pipeline can automatically file change requests (CR) to leave an audit trail. Most organizations use this workflow for standard changes, which means, planned releases.*


- CD Production phase:

*Whether subsystems can be independently deployed, or they need to be assembled into a system, those versioned artifacts are deployed to production as part of this final phase.*

*This is bedrock of "Blue-Green Deployment*. *{{ZDD (zero downtime deployment) is a must to prevent downtime for customers, and should be practiced all the way from test to staging to production. Blue-green deployment is a popular ZDD technique where the new bits are deployed to a tiny cross-section of the population (called “green”), while the bulk is blissfully unaware on “blue” which has the old bits. If push comes to shove, revert everyone back to “blue” and very few customers will be affected, if any. If things look good on “green”, dial everyone up slowly from “blue” to “green”}}*



|**CD Sub-System phase**| **CD System phase**|**CD Production phase**
| :---: | :---:| :---:|
| Workflow | Workflow| Workflow| 
|<img src="assets/CDSubSystemPhas.png" width="400" height="300" border="10">|<img src="assets/CDSSystemPhas.png" width="400" height="300" border="10">| <img src="assets/CDSProductionPhase.png" width="400" height="300" border="10">|
| Click on above Image | Click on above Image :smiley:| Click on above Image :smiley:| 

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
By using best practices of DevSecOps, an end to end secure continuous integration and continuous deployment pipeline is laid out for our customer.  We took the following **23 steps DevSecOps** to achieve our goals:

1. Implement DevSecOps in Product Development Lifecycle
2. Implement Continuous Integration and Continuous Deployment (CI/CD) pipeline with Jenkins (CI Engine)
<br>

3. Integrate Jira (Agile Board) with GitHub (SCM)

4. Integrate Jira with Jenkins (CI Engine - Jenkins as a Code/Pipeline as a Code (JaaC/PaaC))
5. Integrate Jira with Confluence (Wiki)
6. Integrate Jira with Sonarqube (SCAT)

<br>

7. Configure Jenkins for Maven, Wheel & other code build tools (CBT)
8. Integrate Jenkins with Sonarqube (SCAT)
9. Integrate Jenkins with FORTIFY/CHECKMARX (SAST)
10. Integrate Jenkins with Nexus (Artefact Repository Manager)
12. Integrate Jenkins with Docker (Containers/Virtualization - Docker/RKT)
13. Integrate Jenkins with CLAIR (Container Vulnerability Scanner | Conatiner driven Common Vulnerability Scoring System CVSS)
14. Integrate Jenkins with Azure/ AWS (Cloud Service Provider - CSP)
15. Integrate Jenkins with Terraform/ AWS CloudFormation / AZURE Resource Manager / GCP Deployment Manager (IaC Tools)
<br>

16. Configure Jenkins for Ansible (Configuration Management tool for Multiple Environments)
17. Integrate Jenkins with K8S (openShift K8S/ AWS EKS/ AZURE AKS / GCP GKE/ Rancher)
18. Implement Build notification by Integrating Jenkins with emails and slack
19. Integrate Jenkins with FORTIFY/CHECKMARX (DAST)
<br>

20. Implement SIEM Monitoring Tool in Prod
21. Implement System Telemetry Tool in Prod
22. Implement Metering, Billing & Chargeback Tool in Prod
23. Implement ITSM Ticketing system


#### TECH STACK IN AZURE
This solution used following tools, platforms and services:

1. Azure-Public Cloud Platform. Following services are prominently used:
	- Virtual Machine: for hosting Jenkins, SonarQube and Sonartype Nexus Repository Manager
	- Azure Kubernetes Service (AKS): for creating Kubernetes cluster
2. GitHub-for source code management
3. Maven & Wheel-for building java & Python application
4. Junit & PyTest-for unit test cases
5. Jira-for implementing end to end Agile Board & Agile project workflow
6. Jenkins -as CI Engine
7. SonarQube-for static code analysis
9. CheckMarx for SAST & DAST
9. Sonatype Nexus Repository Manager-for storing docker images
10. Clair-for vulnerability scanning of docker images
11. ELK Stack with Prometheus.io + Kubernetes Dashboard for System Telemetry
12. SolarWinds for SIEM
13. Custom ITSM tool
14. Custom Metering, Billing & Chargeback Tool baesed on "API Metering + Customized OSM + CloudBolt C2 Chargeback Software"



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


# Reference
* https://www.atlassian.com/continuous-delivery/principles/continuous-integration-vs-delivery-vs-deployment
* https://www.atlassian.com/continuous-delivery/pipeline
* https://www.atlassian.com/continuous-delivery/software-testing/code-coverage
* https://get.cloudbolt.io/blog/bid/309670/IT-Usage-Metering-and-CloudBolt-C2
