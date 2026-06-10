# 🚀 Deep Dive: Local to GitHub CI/CD Deployment (DevOps Project)

## 👩‍💻 Project Overview

This project demonstrates a complete **DevOps CI/CD workflow** for deploying a static HTML CV website using:

- Git for version control
- GitHub for remote repository hosting
- GitHub Pages for hosting
- GitHub Actions for CI/CD automation
- Linux (WSL Ubuntu) for development environment

The project simulates a real-world deployment pipeline used in cloud engineering environments.

---

## 🎯 Objective

To build and deploy a personal CV website while practicing:

- Git workflow (commit, push, rebase, conflict resolution)
- Remote repository management
- CI/CD pipeline setup
- Automated deployment using GitHub Actions
- Static site hosting using GitHub Pages

---

## 🛠️ Technologies Used

- HTML5
- Git & GitHub
- GitHub Pages
- GitHub Actions (CI/CD)
- Linux (WSL Ubuntu)
- Nano / Vim editor

---

## 🔄 CI/CD Pipeline Architecture
Local Machine → Git Commit → GitHub Repository → GitHub Actions → GitHub Pages → Live Website


## 📄 Key Code Snippets

### 🌐 HTML CV Structure

```html id="html1"
<h1>Adebayo Ganiyat</h1>
<p>Cloud & DevOps | Data Analytics | Customer Support Supervisor</p>

⚙️ GitHub Actions Workflow
name: Deploy to GitHub Pages

on:
  push:
    branches: [ master ]

permissions:
  contents: read
  pages: write
  id-token: write

jobs:
  deploy:
    runs-on: ubuntu-latest

    steps:
      - uses: actions/checkout@v4
      - uses: actions/configure-pages@v4
      - uses: actions/upload-pages-artifact@v3
        with:
          path: ./
      - uses: actions/deploy-pages@v4
🌐 Live Project

👉 Website URL:
https://umuashraf1.github.io/Deep-dive-local-to-git/

🧠 Key DevOps Learnings
Git branching and rebasing
Handling merge conflicts manually
Remote repository synchronization
CI/CD pipeline automation using GitHub Actions
GitHub Pages deployment workflow
Linux command-line workflow in WSL

⚠️ Challenges Solved
Git push rejection (non-fast-forward errors)
Divergent branch history
Merge conflict resolution in index.html
GitHub Actions deployment failure troubleshooting
Workflow configuration debugging

🚀 Future Improvements
Add responsive CSS design (modern CV UI)
Include profile image and sidebar layout
Add project showcase section
Implement automated testing before deployment
Deploy custom domain (e.g. www.mycv.dev)
Expand into full DevOps portfolio project


👩‍💻 Author

Adebayo Ganiyat
Cloud & DevOps | Data Engineering | Business/Data Analytics | Customer Support Supervisor

📌 Project Status

✔ Fully deployed
✔ CI/CD pipeline active
✔ GitHub Pages hosting enabled
✔ Production-ready DevOps workflow implemented


-

