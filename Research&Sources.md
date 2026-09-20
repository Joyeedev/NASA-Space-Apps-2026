# Research & Sources


## 1.Challenge
Create Health Monitoring Software for Astronauts on Space Missions 
-health monitoring software that gathers health indicators and enables astronauts to evaluate and act on the status of their health.

           
## 2.Catagory of Health Risks:
#### 2.1physical health risks
##### 2.2.1 Cardiovascular adaption:https://www.nasa.gov/reference/risk-of-cardiovascular-adaptations EVIDENCE(knowlenge feed korar jonno lagte pare):https://humanresearchroadmap.nasa.gov/evidence/ 
SOLUTION: BP monitor
#### 2.2.2 Altered Immune system:
FINDING 1:https://www.nasa.gov/directorates/esdmd/hhp/immune-risk/?utm_source=chatgpt.com .
FINDING 2:https://www.nasa.gov/reference/risk-of-altered-immune-system-responses/?utm_source=chatgpt.com

SOLUTION: immune system tracker .indicators:
- sleep
- viral activity 
- stress






#### mental mental health risk 


#### psycological helth risks


## 3.OUR PROJECT :
### 1. Symptom Input & Detection
Astronauts describe their problems (e.g., dizziness, fatigue, irregular heartbeat).

The app uses natural language processing (NLP) to interpret the text.

It maps symptoms to possible health risks using a knowledge base (cardiovascular, musculoskeletal, psychological, etc.).
### 2. Risk Identification
The system compares reported symptoms with stored medical knowledge.

It assigns a risk level (low, moderate, high).

Example: “Dizziness + low blood pressure” → flagged as orthostatic intolerance risk.

### 3. Countermeasures & Advice
Provides evidence-based countermeasures (exercise, fluid intake, compression garments).

Suggests motivational advice (e.g., “Stay consistent with treadmill sessions — this helps your heart adapt to microgravity”).

Offers step-by-step guidance astronauts can follow immediately.

### 4. Contributing Factors Analysis
The app explains why the problem might occur:

Fluid shift in microgravity.

Reduced plasma volume.

Lack of exercise.

Sleep disruption.

This helps astronauts understand the root cause, not just the symptom.

### ⚙️ Architecture Overview
Frontend (Web App): Astronauts input symptoms, view dashboards.

Backend (Knowledge Engine):

Symptom database + medical rules.

Machine learning model for risk detection.

Output:

Risk assessment.

Countermeasure recommendations.

Motivational advice.

Contributing factors explanation.

### Full Feature List
#### Chatbot
Conversational assistant for astronauts.

Symptom reporting → risk detection.

Provides countermeasures, motivational advice, and contributing factors.

Explains health risks in simple terms.

#### 📊 Trackers
Cardiovascular Tracker (HR, BP, HRV).

Immune System Tracker

Exercise Tracker (treadmill, cycling, resistance logs).

Nutrition & Hydration Tracker (fluid intake, meals, supplements).

Sleep & Circadian Tracker (rest quality, light exposure).

Psychological Well-being Tracker (stress, mood check-ins).

#### ⏰ Reminders
Medication reminders.

Exercise session reminders.

Hydration reminders.

Sleep hygiene reminders.

#### 🔔 Notifications
🚨 Critical alerts (immediate medical risk).

⚠️ Warnings (potential issues).

✅ Positive reinforcement (progress updates, motivational nudges).

#### 📚 Knowledge Base
Database of symptoms, risks, countermeasures, and contributing factors.

Rule-based logic (no ML/NLP needed initially).

Expandable for future AI integration.

### 🛠️ Infrastructure Blueprint 
#### 1. Frontend (Web App)
Framework: React / Angular / Vue.

Features: Chatbot UI, dashboards, trackers, reminders, notifications.

Runs on astronaut tablets/laptops.

#### 2. Backend (Application Server)
Framework: Node.js / Django / Flask.

Handles:

Symptom → risk mapping (rule-based engine).

Countermeasure retrieval.

Reminder & notification scheduling.

Simple keyword matching for chatbot (e.g., “dizzy” → orthostatic intolerance).

#### 3. Database Layer
Relational DB (PostgreSQL/MySQL):

Tables: Symptoms, Risks, Countermeasures, Contributing Factors, Tracker Logs, Reminders.

NoSQL DB (MongoDB):

Chatbot conversation logs, unstructured notes.

#### 4. Knowledge Engine (Rule-Based)
Instead of ML/NLP, use if-else rules or decision trees:

Example: IF “dizzy” + “low BP” → Risk = Orthostatic intolerance.

Countermeasure = Fluid intake + compression garments.

Contributing factors = Plasma volume reduction.

#### 5. Integration Layer
APIs to connect wearable sensors (HR monitors, BP cuffs, sleep trackers).

Syncs data into trackers automatically.

#### 6. Notification & Reminder System
Scheduler (e.g., Celery, Cron jobs).

Push notifications via web sockets.

Tiered alerts (critical, warning, motivational).

#### 7. Security & Privacy
End-to-end encryption (TLS).

Role-based access control (astronaut vs medical team).

Authentication (OAuth2, JWT).

#### 8. Deployment
Cloud-based (Azure/AWS/GCP): Earth-side medical dashboards.

Local edge server: Onboard spacecraft for offline use.

Sync when communication link is available.




## 4.X factor of our project(that makes out project differnt):




## 5.CHALLANGES OUR PROJECT MIGHT FACE:



### problems:


### Possible solution:


## 6.WORST CASE SENARIOI( critical situations):

### SOLUTION :


# NASA DATASETS

## 🧬 OSD-575 — Inspiration4 Blood Serum Dataset

**Health Area:** ❤️ Cardiovascular | 🛡️ Immune System | 🧪 Metabolic Health

**Description:**
OSD-575 contains blood serum data collected from astronauts participating in the SpaceX Inspiration4 mission. The dataset includes measurements related to metabolic processes and immune/cardiovascular biomarkers before and after spaceflight.

**Project Contribution:**
This dataset can be used to develop machine-learning models for:

* Cardiovascular health monitoring
* Immune-response analysis
* Metabolic health assessment
* Anomaly detection
* Identifying changes between pre-flight and post-flight health states

**Potential ML Models:**

* Random Forest
* XGBoost
* Logistic Regression
* Isolation Forest
* PCA for dimensionality reduction

**NASA Dataset:**
https://osdr.nasa.gov/bio/repo/data/studies/OSD-575

**Source:** NASA Open Science Data Repository (OSDR)

## 🛡️ OSD-570 — Inspiration4 Immune System Dataset

**Health Area:** 🛡️ Immune System | 🧬 Multi-Omics | 🧑‍🚀 Human Spaceflight

**Description:**
OSD-570 contains biological and multi-omic data collected from astronauts during the SpaceX Inspiration4 mission. The dataset provides information that can be used to investigate how human immune-system responses are affected by spaceflight.

**Project Contribution:**
This dataset can be used to develop machine-learning models for:

* Immune-system monitoring
* Detection of abnormal immune responses
* Biomarker analysis
* Pre-flight vs. post-flight comparison
* Feature selection from high-dimensional biological data

**Potential ML Models:**

* Random Forest
* XGBoost
* Logistic Regression
* PCA
* Isolation Forest
* Neural Networks

**NASA Dataset:**
https://osdr.nasa.gov/bio/repo/data/studies/OSD-570



## 🔬 OSD-656 — Inspiration4 Urine & Inflammation Dataset

**Health Area:** 🛡️ Immune System | 🔥 Inflammation | 🧑‍🚀 Human Spaceflight

**Description:**
OSD-656 contains urine-related biological measurements from the SpaceX Inspiration4 mission. The dataset can be used to investigate biological responses and inflammation-related changes associated with human spaceflight.

**Project Contribution:**
This dataset can contribute to:

* Inflammation monitoring
* Immune-health assessment
* Biomarker analysis
* Detection of abnormal biological patterns
* Pre-flight vs. post-flight health comparison

**Potential ML Applications:**

* Classification of biological health states
* Anomaly detection
* Feature importance analysis
* Clustering of astronaut health profiles
* PCA for dimensionality reduction

**Potential ML Models:**

* Random Forest
* XGBoost
* Logistic Regression
* Isolation Forest
* K-Means
* PCA

**NASA Dataset:**
https://osdr.nasa.gov/bio/repo/data/studies/OSD-656


**Important:**
The dataset should be used as a research resource for identifying biological patterns. ML predictions should not be presented as medical diagnoses.




## 🧑‍🚀 OS-826 — NASA Twins Study

**Health Area:** 🧬 Molecular Health | ❤️ Cardiovascular | 🧠 Behavioral | 🛡️ Immune | Long-Duration Spaceflight

**Description:**
The NASA Twins Study investigated physiological, molecular and behavioral changes associated with approximately one year of spaceflight. The study is particularly relevant to understanding health risks during long-duration missions.

**Project Contribution:**
This dataset can contribute to:

* Long-duration astronaut health analysis
* Identification of physiological changes
* Biological baseline analysis
* Personalized health monitoring
* Development of long-duration mission health models

**Potential ML Applications:**

* Time-series analysis
* Anomaly detection
* PCA
* Feature selection
* Clustering
* Predictive modeling

**NASA Dataset:**
https://osdr.nasa.gov/bio/repo/data/experiments/OS-826

**Source:** NASA Open Science Data Repository (OSDR)

**Important Limitation:**
The Twins Study has an important limitation: the flight twin is effectively an **N=1 spaceflight subject**, so it should not be treated as a large supervised ML training dataset by itself.

## ☢️ OS-844 — Radiation, Immune & Neurobehavioral Effects

**Health Area:** ☢️ Radiation | 🛡️ Immune System | 🧠 Brain | 🧠 Behavioral Health

**Description:**
OS-844 investigates how ionizing radiation, simulated microgravity and social isolation can interact to affect oxidative stress, immune regulation, brain function and neurobehavioral/cognitive performance.

**Project Contribution:**
This dataset can contribute to:

* Radiation-response analysis
* Immune-system monitoring
* Behavioral-health analysis
* Cognitive-performance research
* Identification of relationships between multiple spaceflight stressors

**Potential ML Applications:**

* Classification
* Regression
* Random Forest
* XGBoost
* Clustering
* Anomaly detection

**NASA Dataset:**
https://osdr.nasa.gov/bio/repo/data/experiments/OS-844

**Source:** NASA Open Science Data Repository (OSDR)

**Important:**
This study uses animal models and simulated spaceflight conditions. It should therefore be used as supporting research data rather than as a direct human medical prediction dataset.

## ☢️ OSD-719 — Radiation-Induced Immune & Endocrine Responses

**Health Area:** ☢️ Radiation | 🛡️ Immune System | 🧬 Endocrine System

**Description:**
OSD-719 investigates sex-specific immune and endocrine responses to simulated cosmic ionizing radiation. The study uses radiation exposures designed to represent space-relevant galactic cosmic-ray conditions.

**Project Contribution:**
This dataset can contribute to:

* Radiation-response modeling
* Immune-response analysis
* Biological risk analysis
* Sex-specific response analysis
* Biomarker identification

**Potential ML Applications:**

* Classification
* Feature selection
* Random Forest
* XGBoost
* PCA
* Clustering

**NASA Dataset:**
https://osdr.nasa.gov/bio/repo/data/studies/OSD-719

**Source:** NASA Open Science Data Repository (OSDR)

**Important:**
This is a mouse study, so ML results should be presented as biological research findings rather than direct predictions of astronaut health.

## ❤️ OSD-591 — Space Radiation & Cardiovascular Health

**Health Area:** ☢️ Radiation | ❤️ Cardiovascular System | 🛡️ Immune Response

**Description:**
OSD-591 investigates the effects of space-relevant radiation exposure on cardiac function and structure, including immune-cell infiltration in a mouse model.

**Project Contribution:**
This dataset can contribute to:

* Radiation-related cardiovascular research
* Cardiac-response analysis
* Immune-cell response analysis
* Radiation dose-response modeling
* Identification of biological patterns associated with cardiovascular effects

**Potential ML Applications:**

* Regression
* Classification
* Random Forest
* XGBoost
* Dose-response modeling
* Anomaly detection

**NASA Dataset:**
https://osdr.nasa.gov/bio/repo/data/studies/OSD-591

**Source:** NASA Open Science Data Repository (OSDR)

**Important:**
The dataset uses a mouse model and should be treated as supporting biological research rather than a direct human clinical prediction dataset.


## ❤️ OS-816 — Microgravity, Inflammation & Circulatory Function

**Health Area:** ❤️ Cardiovascular | 🛡️ Immune System | 🧬 Inflammation

**Description:**
OS-816 investigates how simulated microgravity can cause systemic inflammation and affect circulatory function and structure. NASA identifies cardiovascular physiology and immunology as the main research areas.

**Project Contribution:**
This dataset can contribute to:

* Cardiovascular health monitoring
* Inflammation analysis
* Immune-system monitoring
* Microgravity-related health research
* Analysis of relationships between immune and cardiovascular systems

**Potential ML Applications:**

* Classification
* Regression
* Random Forest
* XGBoost
* Correlation analysis
* Anomaly detection

**NASA Dataset:**
https://osdr.nasa.gov/bio/repo/data/experiments/OS-816

**Source:** NASA Open Science Data Repository (OSDR)

**Important:**
The study uses simulated microgravity rather than direct long-duration human spaceflight measurements.

## 🦴 OSD-919 — Spaceflight Bone & Immune System Dataset

**Health Area:** 🦴 Bone Health | 🛡️ Immune System | 🧬 Single-Cell Biology

**Description:**
OSD-919 contains single-cell RNA sequencing data from spaceflight and control conditions. The study investigates systemic effects of spaceflight on tissues, including changes relevant to bone, extracellular matrix and immune-system regulation.

**Project Contribution:**
This dataset can contribute to:

* Bone-health research
* Spaceflight-related bone-loss analysis
* Immune-system analysis
* Single-cell feature extraction
* Identification of biological changes caused by spaceflight

**Potential ML Applications:**

* PCA
* Clustering
* Random Forest
* Neural Networks
* Feature selection
* Cell-type classification

**NASA Dataset:**
https://osdr.nasa.gov/bio/repo/data/studies/OSD-919

**Source:** NASA Open Science Data Repository (OSDR)

**Dataset Type:**
Single-cell RNA sequencing


