# security_product_project
# Problem statements solution of Accoknox india private limited technical round

# 1.Problem Statement 1:

# 📄 Product Requirement and Low-Fidelity Wireframes

### 🔐 Project Overview
This project focuses on building a security product that scans **container images** and displays findings related to **vulnerabilities**. It allows users to understand which images have vulnerabilities, especially those classified as **critical** or **high**, helping them prioritize which images to fix.

---

## 📌 Problem Statement
Container images may contain applications with various dependencies, and these can introduce vulnerabilities. Given that a user might be managing **thousands of container images**, it's essential to design a system that:

- Clearly shows **which images** are vulnerable.
- Communicates **severity levels**.
- Provides **filtering/searching** to quickly locate high-risk images.

---

## 🧾 Product Requirements Document (PRD)

### 🎯 Goals
- Enable users to **view**, **filter**, and **prioritize** vulnerabilities.
- Provide **actionable insights** (e.g., remediation steps).
- Support **large-scale** environments with thousands of images.

### 👥 Target Users
- Security Engineers
- DevOps Engineers
- Platform Admins

### ✨ Key Features
| Feature | Description |
|--------|-------------|
| Dashboard | Displays container image list with vulnerability stats |
| Severity Filter | Filter images by vulnerability severity (Low, Medium, High, Critical) |
| Image Search | Quickly search by image name or tag |
| Detail View | View CVE-level details with fix suggestions |
| Pagination | Efficient handling of large image repositories |

### 📐 Non-Functional Requirements
- Scalable to handle >10K container images.
- Responsive web UI (Desktop + Mobile).
- Secure with role-based access.

---

## 🖼️ Low-Fidelity Wireframes

The wireframes illustrate the following UI components in grayscale:

### 🧭 1. Dashboard View

- **Search bar** to filter by image name.
- **Filter buttons** for severity levels.
- **Table View** with image name, total vulnerabilities, severity breakdown.
- **Action Buttons** to “View Details” for deeper analysis.


### 🔎 2. Image Detail View (Described in layout)

- Image metadata (e.g., name, version).
- Table of vulnerabilities:

# 2. Problem Statement 2:

# 🔍 Kubernetes Security Scan

### 📦 Overview
This project sets up a **local Kubernetes cluster** and performs a **security scan** using a tool like **Kubescape**, generating a structured list of vulnerabilities, misconfigurations, and policy violations in the form of a **JSON report**.

---

## 🧠 Problem Statement

> Set up a local Kubernetes cluster and scan it for security issues using tools such as **Kubescape**, **Kube-bench**, or any similar K8s security scanning tool.  
>  
> Output the findings in **JSON format**.

---

## 🚀 Deliverables

- ✅ Local Kubernetes cluster (e.g., Minikube, Kind, or K3s)
- ✅ Security scanning tool installed (e.g., Kubescape)
- ✅ A `findings.json` file containing scan results

---

## 🧰 Tools & Technologies

| Category | Tool |
|----------|------|
| K8s Cluster | Minikube |
| Scanner | Kubescape |
| OS | Windows (WSL) |
| Output Format | JSON |

# 3. Problem Statement 3:
  
# 🕒 GoLang Web App: Date & Time + K8s Deployment

### 📦 Overview
This project demonstrates:
- A **GoLang web server** displaying the current date and time.
- Containerization using **Docker** and pushing the image to **DockerHub**.
- Declarative deployment of the app to **Kubernetes** with **2 replicas**.
- Exposure to the **internet (WAN)** using a **LoadBalancer** or **Ingress**.

---
