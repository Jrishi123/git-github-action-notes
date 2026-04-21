# 🚀 GitHub Actions Notes (Beginner → DevOps Level)

## 📌 What is GitHub Actions?
GitHub Actions is a CI/CD tool provided by GitHub to automate workflows like build, test, and deployment.

---

## 🎯 Why GitHub Actions?
- Automates CI/CD pipelines
- Integrated with GitHub
- Supports multiple languages and platforms
- Reduces manual work

---

## 🧱 Key Concepts

### 🔹 Workflow
A workflow is an automated process defined in a YAML file.

📁 Location:
.github/workflows/

---

### 🔹 Event
Triggers that start workflows.

Examples:
- push
- pull_request
- schedule

---

### 🔹 Job
A job is a set of steps that run on a runner.

---

### 🔹 Step
Individual task inside a job.

---

### 🔹 Runner
A machine where the workflow runs.

Example:
runs-on: ubuntu-latest

---

## ⚙️ Basic Workflow Example

```yaml
name: First Workflow

on:
  push:
    branches:
      - main

jobs:
  build:
    runs-on: ubuntu-latest

    steps:
      - name: Checkout Code
        uses: actions/checkout@v3

      - name: Run Command
        run: echo "Hello, GitHub Actions 🚀"