# Black IT Academy - DevSecOps Sample Repository

A hands-on learning repository designed for Black IT Academy members to explore DevSecOps practices in a real-world development environment.

## 🎯 Purpose

This repository serves as a practical learning environment for Black IT Academy members interested in DevSecOps. It demonstrates industry-standard practices including automated security scanning, CI/CD pipelines, and collaborative development workflows.

## 📦 What's Included

### 🌐 Simple Landing Page Application
- **Technology Stack**: Vanilla HTML, CSS, and JavaScript
- **Purpose**: Clean, responsive landing page for the Black IT Academy
- **Structure**: Standard web application with modern styling and interactive elements

### 🔄 GitHub Actions Pipeline
- **Automated Workflows**: Triggers on every push to any branch
- **Quality Assurance**: Runs tests and builds automatically
- **Integration**: Seamlessly connected to SonarQube for security analysis

### 🔒 SonarQube SAST Security Scanning
- **Security Analysis**: Static Application Security Testing (SAST) on every commit
- **Code Quality**: Automated code quality and vulnerability detection
- **Platform**: Connected to SonarQube Free Edition (SonarCloud)
- **Reports**: Detailed security and quality reports on pull requests

### 🌿 Branching Strategy & PR Workflow
- **Branch Types**: 
  - `main` - Production-ready code
  - `dev` - Development integration branch
  - `feature/*` - New feature development
  - `hotfix/*` - Critical bug fixes
- **PR Approval Process**: Simulates real-world development environment with required reviews

## 🚀 How to Use

### Getting Started
1. **Fork this repository** to your GitHub account
2. **Clone your fork** locally:
   ```bash
   git clone https://github.com/YOUR-USERNAME/DevSecOps.git
   cd DevSecOps
   ```

### Making Changes
1. **Create a new branch** for your work:
   ```bash
   # For new features
   git checkout -b feature/your-feature-name
   
   # For bug fixes
   git checkout -b hotfix/your-fix-name
   ```

2. **Make your changes** to the HTML, CSS, or JavaScript files

3. **Commit and push** your changes:
   ```bash
   git add .
   git commit -m "Add: your descriptive commit message"
   git push origin your-branch-name
   ```

### What to Expect

#### ✅ Automated Checks
When you push code or create a pull request, you'll see:
- **GitHub Actions workflow** runs automatically
- **SonarQube scan** analyzes your code for:
  - Security vulnerabilities
  - Code quality issues
  - Best practice violations
  - Maintainability concerns

#### 📊 Results & Feedback
- **Pull Request Comments**: SonarQube automatically comments on PRs with analysis results
- **Quality Gate**: Your PR must pass quality standards to be merged
- **Workflow Status**: Green checkmarks indicate successful builds and scans

#### 🔄 Review Process
- Create pull requests to merge changes into `main` or `dev`
- PR approval required before merging (simulates real-world workflows)
- All automated checks must pass

### Example Workflow
```bash
# 1. Create feature branch
git checkout -b feature/update-homepage

# 2. Make changes to index.html or styles.css
# 3. Commit changes
git commit -m "Update: homepage hero section styling"

# 4. Push to GitHub
git push origin feature/update-homepage

# 5. Create Pull Request on GitHub
# 6. Wait for automated checks to complete
# 7. Address any SonarQube issues if needed
# 8. Get approval and merge
```

## 🛠️ Technical Details

- **CI/CD**: GitHub Actions workflows in `.github/workflows/`
- **Security Config**: SonarQube settings in `sonar-project.properties`
- **Quality Gates**: Automated quality and security thresholds
- **Branch Protection**: Configured to require PR reviews and passing checks

## 🤝 Join the Community

### Discord
Connect with fellow DevSecOps learners: [Join our Discord](https://discord.gg/45P6d53VsN)

### Follow Black IT Academy
- **LinkedIn**: [Black IT Academy Company Page](https://www.linkedin.com/company/black-it-academy/)
- **TikTok**: [@blackitacademy](https://www.tiktok.com/@blackitacademy?_t=ZP-8yJ57nwN8Ws&_r=1)

## 📚 Learning Outcomes

By working with this repository, you'll gain hands-on experience with:
- Git branching strategies and collaborative workflows
- Automated security scanning and SAST tools
- CI/CD pipeline configuration and management
- Code quality gates and automated testing
- Industry-standard DevSecOps practices