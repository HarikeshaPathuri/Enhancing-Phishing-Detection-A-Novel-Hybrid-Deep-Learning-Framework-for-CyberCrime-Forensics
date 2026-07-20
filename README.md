# 🛡️✨ Enhancing Phishing Detection: A Novel Hybrid Deep Learning Framework for Cybercrime Forensics 🔍🕵️‍♂️

> 🌐 A Django-powered web platform that hunts down phishing, malware, and defaced URLs in real time — armed with an ensemble of machine learning ⚙️ and deep learning 🧠 models. Built with 💙 as a Major Project (B.Tech CSE – AI & ML) at Sree Chaitanya Institute of Technological Sciences, JNTUH.

---

## 📌✨ Overview

🎣 Phishing is one of the most widespread cybercrimes today — tricking people into handing over financial and personal data through deceptive URLs, spoofed emails, and fake websites.

This project delivers a **web-based phishing URL detection system** 🕸️ that instantly classifies any submitted URL into one of several threat categories:

🟢 **Non-Phishing** | 🔴 **Phishing** | 🦠 **Malware** | 🎭 **Defacement**

...while giving administrators a slick 📊 dashboard to train models, compare classifier performance, and keep an eye on users. 👀

💡 The system draws inspiration from the IEEE Access paper *"Enhancing Phishing Detection: A Novel Hybrid Deep Learning Framework for Cybercrime Forensics"* (Alsubaei, Almazroi & Ayub, 2024), which proposes a ResNeXt + GRU hybrid model (RNT) with SMOTE-based class balancing ⚖️ and autoencoder-ResNet feature extraction 🧬.

---

## 🎯 Objectives

- ⚡ Detect phishing/malicious URLs in real time with high accuracy
- ⚖️ Handle class imbalance in phishing datasets effectively
- 🧑‍💻 Provide a smooth, role-based web interface for admins and end users
- 📈 Compare multiple ML/DL classifiers and visualize their performance
- 🕵️ Support digital forensics use cases with downloadable prediction reports

---

## 🧩✨ Key Features

### 👤 Remote User Module
- 🔐 Secure registration and login
- 🔎 Submit a URL and get an **instant prediction**
- 🪪 View personal profile details
- 📄 View phishing detection prediction results

### 🛠️ Service Provider (Admin) Module
- 🔑 Secure admin login
- 🏋️ Train & test URL datasets
- 📊 View model accuracy as **bar charts** 📶 and **pie charts** 🥧
- 📉 View prediction results and phishing detection ratio
- ⬇️ Download predicted datasets
- 👥 View and manage all registered remote users

---

## 🏗️ System Architecture

A clean client-server setup 🖥️↔️🖧, with a central web server handling requests from both **Service Providers** 🛠️ and **Remote Users** 👤, backed by a MySQL database 🗄️ storing datasets, predictions, and user records.

```
👤 Remote User      ──┐
                       ├──► 🌐 Web Server ──► 🧠 ML/DL Models ──► 🗄️ MySQL Database
🛠️ Service Provider ──┘
```

📐 Full architecture, data flow diagrams, use case, class, and sequence diagrams are documented in the project report (`/docs`).

---

## 🧠⚡ Algorithms & Models Used

| Category | Algorithms |
|---|---|
| 🌳 Classical ML | Decision Tree, Random Forest, Logistic Regression, Naive Bayes, K-Nearest Neighbors (KNN), Support Vector Machine (SVM), Gradient Boosting, SGD Classifier |
| 🧠 Deep Learning | Recurrent Neural Network (RNN) |
| ⚖️ Data Balancing | SMOTE (Synthetic Minority Oversampling Technique) |

📊 Model performance is benchmarked and visualized live in the admin dashboard — Gradient Boosting, RNN, Logistic Regression, and SGD Classifier go head-to-head! 🥊

---

## 🛠️✨ Tech Stack

| Layer | Technology |
|---|---|
| 🐍 Language | Python |
| 🌐 Web Framework | Django |
| 🎨 Frontend | HTML, CSS, JavaScript |
| 🗄️ Database | MySQL (via WAMP Server) |
| 🤖 ML/DL Libraries | Scikit-learn, RNN implementation |
| 📊 Visualization | Bar Chart / Pie Chart (in-app analytics) |

---

## 📂 Project Structure (suggested)

```
├── phishing_detection/        # ⚙️ Django project settings
├── remote_user/               # 👤 Remote user app (registration, prediction)
├── service_provider/          # 🛠️ Admin app (training, analytics, user management)
├── static/                    # 🎨 CSS, JS, images
├── templates/                 # 🖼️ HTML templates
├── datasets/                  # 📁 URL datasets used for training/testing
├── docs/                      # 📖 Project report, diagrams, screenshots
├── requirements.txt
└── manage.py
```

> ✏️ Update this section to match your actual repository layout.

---

## ⚙️🚀 Installation & Setup

```bash
# 1️⃣ Clone the repository
git clone https://github.com/HarikeshaPathuri/<your-repo-name>.git
cd <your-repo-name>

# 2️⃣ Create and activate a virtual environment
python -m venv venv
source venv/bin/activate      # On Windows: venv\Scripts\activate

# 3️⃣ Install dependencies
pip install -r requirements.txt

# 4️⃣ Configure the MySQL database
# Update DATABASES settings in settings.py with your MySQL credentials

# 5️⃣ Apply migrations
python manage.py makemigrations
python manage.py migrate

# 6️⃣ Run the development server ✨
python manage.py runserver
```

🌐 Visit `http://127.0.0.1:8000` in your browser and watch the magic happen! ✨

---

## 📊🏆 Results

- 🧪 Multiple classifiers were trained and evaluated on real-world phishing URL datasets
- 📈 Model accuracy is visualized via bar and pie charts for easy comparison
- ⚡ The system successfully classifies URLs into **Phishing** 🔴, **Non-Phishing** 🟢, **Malware** 🦠, and **Defacement** 🎭 categories — in real time!

---

## 🔮✨ Future Scope

- 🧬 Integrate the full ResNeXt + GRU (RNT) hybrid deep learning model with Jaya optimization (RNT-J), as proposed in the referenced research
- 🧠 Incorporate autoencoder + ResNet (EARN) based feature extraction for even sharper accuracy
- 📧 Extend detection to email-based phishing and real-time browser plugin integration
- ☁️ Deploy on cloud infrastructure for scalable, production-grade forensic use

---

## 👥💫 Team

| Name | Hall Ticket No. |
|---|---|
| Muthyam Pranavi | 22TR1A6639 |
| Nagunuri Deekshitha | 22TR1A6640 |
| **✨ Pathuri Harikesha** | 22TR1A6645 |
| Marri Yashwanth | 22TR1A6634 |

🎓 **Project Guide:** K. Sireesha, Assistant Professor
🏛️ **Department:** Computer Science & Engineering (AI & ML)
🏫 **Institution:** Sree Chaitanya Institute of Technological Sciences, Karimnagar (Affiliated to JNTUH)

---

## 📖 Reference

This project is conceptually inspired by:
> F. S. Alsubaei, A. A. Almazroi and N. Ayub, "Enhancing Phishing Detection: A Novel Hybrid Deep Learning Framework for Cybercrime Forensics," *IEEE Access*, vol. 12, 2024.

---

## 📄 License

🎓 This project was developed for academic purposes as part of a B.Tech Major Project. Feel free to fork and build upon it for learning purposes. ⭐ If it helped you, consider giving it a star!
