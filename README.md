# SitSaay (စစ်ဆေး)

An AI-powered cybersecurity platform and application dedicated to creating a "Zero Victim" digital environment by proactively detecting and preventing digital fraud, phishing, and AI-generated deepfakes.

---

## 📌 Project Overview
With the rapid rise of digital financial scams and online deception, cybersecurity has become a critical necessity for everyday internet users. **SitSaay** is designed to act as a shield against these digital threats, providing real-time verification tools directly at the user's fingertips.

### 🔴 The Problem
* **Sophisticated Phishing:** Attackers use complex URL redirection and look-alike domains to steal user credentials.
* **Social Engineering Fraud:** Malicious links and deceptive messages target vulnerable individuals through social applications.
* **Deepfakes & Visual Forgery:** The spread of AI-generated fake media makes manual verification almost impossible for general users.

### 🟢 The Solution
* A comprehensive, lightweight security app that leverages advanced AI models to instantaneously analyze URLs, check file/image integrity, and flag potential cyber risks before any harm occurs.

---

## 🛠️ Tech Stack & Architecture
The system was architected focusing on responsiveness, high throughput, and robust security principles:

* **Frontend/Mobile:** React (Web Dashboard) / Kotlin & Java (Android Mobile Application)
* **Backend Framework:** Node.js / Express or Python-based API gateway
* **AI Engine:** Google Gemini AI integration for predictive link analysis, textual pattern recognition, and anomaly detection
* **Database & Auth:** Firebase Services / Secure Manual Database integration

### Conceptual System Workflow
1. **Input Layer:** The user inputs a suspicious URL, copies a fishy text message, or uploads a doubtful image/screenshot into the SitSaay application.
2. **Analysis Layer (Gemini AI):** The system passes the payload to the backend where Gemini AI evaluates semantic contextual patterns, URL structures, and metadata anomalies.
3. **Verification Layer:** The application cross-references threat data against real-time blacklists and previous fraud logs.
4. **Actionable Output:** Within seconds, the user receives a clean, color-coded safety rating (Safe / Warning / Dangerous) along with detailed risk flags.

---

## 🗄️ Database Design (Conceptual Schema)
The data layer is structured to track scanned logs and maintain dynamic threat intelligence data efficiently.

### 1. Users Table
| Column Name | Data Type | Description |
| :--- | :--- | :--- |
| `user_id` | INT (PK) | Unique identifier for each registered user |
| `username` | VARCHAR | User's identifier |
| `created_at` | TIMESTAMP | Account registration date |

### 2. Threat_Logs Table
| Column Name | Data Type | Description |
| :--- | :--- | :--- |
| `log_id` | INT (PK) | Unique identifier for the scan record |
| `user_id` | INT (FK) | References the user who performed the scan |
| `scan_type` | VARCHAR | Type of payload scanned (`URL`, `TEXT`, `IMAGE`) |
| `scanned_content` | TEXT | The actual content/link analyzed |
| `risk_level` | VARCHAR | Calculated threat level (`LOW`, `MEDIUM`, `HIGH`) |
| `scanned_at` | TIMESTAMP | Timestamp of the analysis |

---

## 🚀 Key Features & Functionalities
* **AI-Driven URL & Link Analysis:** Instantly checks short links and masked URLs to reveal their true destination and threat vectors using Gemini AI models.
* **Zero-Victim Fraud Prevention:** A proactive scanning flow that intercepts dangerous inputs before the user interacts with malicious platforms.
* **Contextual Fraud Detection:** Analyzes suspicious chat messages or SMS text for phishing patterns and manipulative language common in online scams.
* **Clean & Dynamic User Interface:** Built with intuitive navigation paths, making cybersecurity tools accessible to non-tech-savvy users.

---

## 🎯 Key Takeaways & Learnings
Designing SitSaay provided invaluable engineering insights:
* **AI Integration:** Gained practical knowledge on structuring reliable prompts and handling JSON responses from LLMs (Gemini AI) for security classification tasks.
* **Security-First Architecture:** Learned the importance of sanitizing inputs and designing architectures that prioritize user data privacy.
* **Defensive System Design:** Understood how to model database schemas that quickly flag malicious patterns while scaling gracefully.

---
📧 **Contact:** Feel free to connect for internship opportunities or collaborations!
* **Email:** swezinmyat164@gmail.com
* **LinkedIn:** swezinmyat164@gmail.com
