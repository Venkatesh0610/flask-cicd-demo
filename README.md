# Flask CI/CD Pipeline on AWS (Manual vs CI/CD)

This repository demonstrates a **practical, step-by-step implementation of deploying a Flask application on AWS EC2**, both **with and without CI/CD**, using **GitHub Actions**.

The goal of this project is to help beginners and intermediate developers clearly understand:

* How manual deployment works
* Why CI/CD is important
* How GitHub Actions automates real-world deployments
<img width="1536" height="1024" alt="cicd pipeline 1" src="https://github.com/user-attachments/assets/cc825800-0398-44bb-a785-568d742097eb" />

---

## 🚀 What This Project Covers

### ✅ Without CI/CD (Manual Deployment)

* Create a basic Flask application
* Push code to GitHub
* Launch an AWS EC2 instance
* SSH into EC2
* Manually set up environment and dependencies
* Run the Flask app using Gunicorn
* Access the application via EC2 public IP

### ✅ With CI/CD (Automated Deployment)

* Use the same Flask application
* Configure a **self-hosted GitHub Actions runner** on EC2
* Create a CI/CD workflow using GitHub Actions
* Store sensitive values using GitHub Secrets
* Automatically deploy the app on every GitHub push

---

## 🛠 Tech Stack Used

* **Python**
* **Flask**
* **Gunicorn**
* **AWS EC2 (Ubuntu)**
* **Git & GitHub**
* **GitHub Actions (CI/CD)**

---

## 📂 Project Structure

```
flask-cicd-demo/
│── main.py
│── requirements.txt
│── .gitignore
│── .github/
│   └── workflows/
│       └── cicd.yaml
```

---

## ⚙️ How the CI/CD Pipeline Works

1. Developer updates Flask code locally
2. Code is pushed to GitHub
3. GitHub Actions workflow is triggered
4. Self-hosted runner on EC2 executes the workflow
5. Dependencies are installed
6. Flask app is deployed automatically
7. Application is accessible via EC2 public IP

---

## 🔐 GitHub Secrets Used

The following secrets are configured in **GitHub → Settings → Secrets and variables → Actions**:

* `EC2_HOST` → EC2 public IPv4 address
* `EC2_SSH_KEY` → Private key (.pem file content)

---

## 🌐 Accessing the Application

After deployment, access the Flask app using:

```
http://<EC2_PUBLIC_IP>:5000
```

---

## 📘 Detailed Explanation

For a **detailed explanation with screenshots, flow diagrams, and step-by-step commands**, please refer to my **Medium blog**:

👉 [***Medium Blog Link***](https://medium.com/@avenkatesh0610/a74180283651)

---

## 🎥 Video Content

A **full YouTube video walkthrough** of this project will be released soon, covering:

* Manual deployment
* CI/CD setup
* Common mistakes
* Real-world best practices

Stay tuned and [**SUBSCRIBE**](https://www.youtube.com/@avenkatesh0610) for updates 🚀

---

## 💡 Why This Project?

* Beginner-friendly
* Real-world CI/CD workflow
* Interview-ready project
* Clear comparison of **CI/CD vs No CI/CD**

---

## ⭐ Support

If you found this helpful:

* Star ⭐ the repository
* Follow the blog for more content
* Comment if you want a **GCP CI/CD version** in the future

Happy building! 🚀
