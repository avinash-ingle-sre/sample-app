# 🚀 GKE CI/CD Pipeline Project

## 📌 Project Overview
This project sets up a complete CI/CD pipeline for a Go application on **Google Kubernetes Engine (GKE)**. 
It automates the build and deployment process using **Cloud Build** and **Artifact Registry**.

---

## 🏗️ Architecture Flow

[ Developer ]  --->  ( Pushes Code to GitHub )
      |
      v
[ Cloud Build Trigger ]
      |
      +---> 1. Builds Docker Image 🐳
      |
      +---> 2. Pushes to Artifact Registry 📦
      |
      +---> 3. Deploys to GKE Cluster ☸️
            (Updates Dev or Prod Namespace)

---

## 🛠️ Key Technologies Used
* **Google Cloud Platform (GCP)**
* **Google Kubernetes Engine (GKE)**
* **Cloud Build** (CI/CD)
* **Artifact Registry** (Docker Images)
* **Git & GitHub** (Version Control)
* **Go Lang** (Application)

---

## ✅ Tasks Completed
1.  **Setup:** Created GKE Cluster & Artifact Registry.
2.  **Automation:** Configured Cloud Build Triggers for 'Main' and 'Dev' branches.
3.  **Deployment:** * Deployed **v1.0** to Production.
    * Deployed **v2.0** (Red Version) to Development.
4.  **Rollback:** Successfully rolled back Production from v2.0 to v1.0 due to issues.
5.  **GitOps:** Synced the GitHub repository with the live cluster state.

---

## 🚀 How to Run
1.  **Clone the repo:**
    `git clone https://github.com/YOUR-USERNAME/sample-app.git`

2.  **Switch to branch:**
    `git checkout dev`

3.  **Push changes to trigger pipeline:**
    `git add .`
    `git commit -m "Update feature"`
    `git push origin dev`

---
*Created by Avinash Ingle - DevOps/SRE Engineer*
