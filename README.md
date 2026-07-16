# IoT Security Risk Management for Small-Scale IoT Systems

![GitHub](https://img.shields.io/badge/Project-IoT%20Security-blue)
![University](https://img.shields.io/badge/University-Van%20Hien-green)
![Course](https://img.shields.io/badge/Course-IoT%20Security-orange)
![License](https://img.shields.io/badge/License-Educational-lightgrey)

---

# Đề tài 35 - Quản lý rủi ro bảo mật cho hệ thống IoT quy mô nhỏ

## Course

IoT Security (INT570)

## University

Van Hien University

## Lecturer

Ho Nhut Minh

## Author

Vo Nguyen Duyen

Student ID: 231A010722

Academic Year: 2025–2026

---

# Project Description

This project presents a lightweight security risk management framework for a small-scale Internet of Things (IoT) laboratory.

The study focuses on identifying critical assets, analyzing threats and vulnerabilities, evaluating security risks, constructing a Risk Register, designing a 5×5 Risk Matrix, and proposing appropriate mitigation strategies.

The framework is suitable for small organizations, educational laboratories and home IoT environments.

---

# Objectives

- Build an IoT asset inventory.
- Identify threats and vulnerabilities.
- Evaluate risks using Likelihood × Impact.
- Build a Risk Register.
- Create a 5×5 Risk Matrix.
- Develop a Risk Treatment Plan.
- Create a periodic Security Checklist.
- Compare the methodology with international security standards.

---

# IoT System Architecture

The laboratory includes:

- IP Camera
- Temperature Sensor
- Smoke Sensor
- PIR Sensor
- Smart Door Lock
- Gateway (Node-RED)
- Wi-Fi Router
- Cloud Dashboard
- Mobile Application

```text
IP Camera
      │
Temperature Sensor
      │
Smoke Sensor
      │
PIR Sensor
      │
Gateway (Node-RED)
      │
Wi-Fi Router
      │
Cloud Dashboard
      │
Mobile Application
```

---

# Repository Structure

```text
IoT-Security-Risk-Management
│
├── README.md
│
├── report
│   ├── Bao_cao_tieu_luan.docx
│   └── Bao_cao_tieu_luan.pdf
│
├── images
│   ├── figure3_1_nist.png
│   ├── figure3_2_owasp.png
│   ├── figure4_1_architecture.png
│   ├── figure5_1_risk_matrix.png
│   ├── figure5_2_risk_register.png
│   └── figure5_3_node_red.png
│
├── results
│   ├── 01_asset_inventory.csv
│   ├── 02_risk_register.csv
│   ├── 03_risk_matrix.csv
│   ├── 04_risk_treatment_plan.csv
│   └── 05_security_checklist.csv
│
└── references
    └── references.md
```

---

# Main Contents

The repository contains:

## Asset Inventory

Identify critical assets of the IoT laboratory.

## Risk Register

Security risks including:

- Assets
- Threats
- Vulnerabilities
- Likelihood
- Impact
- Risk Score
- Risk Priority

## 5×5 Risk Matrix

Visual representation of security risks.

## Risk Treatment Plan

Top five risks and mitigation strategies.

## Security Checklist

Periodic inspection checklist for maintaining system security.

---

# Project Outputs

The project successfully produced:

- Asset Inventory
- Risk Register (17 security risks)
- 5×5 Risk Matrix
- Risk Treatment Plan
- Security Checklist
- Node-RED Gateway Architecture

---

# Figures

The report contains six figures:

- Figure 3.1 – NIST SP 800-30 Risk Management Process
- Figure 3.2 – OWASP IoT Top 10
- Figure 4.1 – IoT System Architecture
- Figure 5.1 – 5×5 Risk Matrix
- Figure 5.2 – Risk Register
- Figure 5.3 – Node-RED Gateway Architecture

---

# Security Standards Used

This project is based on:

- OWASP IoT Project
- OWASP ISVS
- OWASP ISTG
- NIST SP 800-30 Rev.1
- ISO/IEC 27005

---

# References

- OWASP IoT Security Verification Standard (ISVS)
- OWASP IoT Security Testing Guide (ISTG)
- OWASP Internet of Things Project
- NIST SP 800-30
- ISO/IEC 27005
- Node-RED

---

# Limitations

- Educational laboratory model.
- No penetration testing on production systems.
- No personal or sensitive data.
- Risk evaluation based on a simulated environment.

---

# Future Work

Future improvements include:

- Deploying the framework on a real IoT laboratory.
- Automating configuration auditing.
- Integrating CVSS scoring.
- Developing a web dashboard for continuous monitoring.
- Automating security checklist verification.

---

# Acknowledgements

Special thanks to

**Ho Nhut Minh**

for guidance throughout this project.

Thanks to

Van Hien University

for providing the learning environment and resources.

---

# License

This repository is created for educational and research purposes only.

© 2026 Vo Nguyen Duyen

All Rights Reserved.
