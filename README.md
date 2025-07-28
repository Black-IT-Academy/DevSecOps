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

## 📝 Step-by-Step Guide: Committing Changes & Creating Pull Requests

### 1. Setting Up Your Environment
```bash
# Clone the repository (if you haven't already)
git clone https://github.com/YOUR-USERNAME/DevSecOps.git
cd DevSecOps

# Check current branch
git branch

# Make sure you're up to date
git pull origin main
```

### 2. Creating and Switching to a New Branch
```bash
# Create and switch to a new feature branch
git checkout -b feature/your-feature-name

# Or for a hotfix
git checkout -b hotfix/fix-description

# Verify you're on the new branch
git branch
```

### 3. Making Changes
- Edit your HTML, CSS, or JavaScript files using your preferred code editor
- Save your changes
- Test your changes locally by opening `index.html` in a browser

### 4. Staging and Committing Changes
```bash
# Check what files have been modified
git status

# Stage specific files
git add index.html
git add styles.css

# Or stage all changes at once
git add .

# Commit with a descriptive message
git commit -m "Add: new hero section with animations"

# Good commit message examples:
# "Fix: navigation menu mobile responsiveness"
# "Update: color scheme to match brand guidelines"
# "Add: contact form validation"
```

### 5. Pushing Changes to GitHub
```bash
# Push your branch to GitHub
git push origin feature/your-feature-name

# If it's your first push on this branch, Git will show you the exact command
```

### 6. Creating a Pull Request (PR)
1. **Go to GitHub**: Navigate to your forked repository on GitHub
2. **Find your branch**: GitHub will usually show a banner suggesting to create a PR
3. **Click "Compare & pull request"** or go to the "Pull requests" tab and click "New pull request"
4. **Select branches**:
   - **Base**: `main` (or `dev` if contributing to development)
   - **Compare**: `feature/your-feature-name`
5. **Fill out PR details**:
   ```
   Title: Add hero section animations
   
   Description:
   - Added smooth fade-in animations to hero section
   - Improved mobile responsiveness
   - Updated color contrast for accessibility
   
   Testing:
   - Tested on Chrome, Firefox, Safari
   - Verified mobile responsiveness on multiple devices
   ```
6. **Click "Create pull request"**

### 7. After Creating Your PR
**What happens automatically:**
- ✅ GitHub Actions workflow runs
- 🔍 SonarQube scans your code
- 📊 Quality report appears in PR comments
- 🚦 Status checks show pass/fail results

**What you should do:**
- Monitor the PR for any failed checks
- Address any SonarQube issues if they appear
- Respond to reviewer feedback
- Make additional commits if needed (they'll automatically update the PR)

### 8. Making Changes After PR Creation
If you need to make changes after creating the PR:
```bash
# Make sure you're on your feature branch
git checkout feature/your-feature-name

# Make your changes and commit them
git add .
git commit -m "Fix: address SonarQube security recommendations"

# Push the updates
git push origin feature/your-feature-name

# The PR will automatically update with your new commits
```

### 9. PR Review Process
- Wait for automated checks to complete (usually 2-5 minutes)
- Address any SonarQube security or quality issues
- Request review from maintainers or peers
- Make requested changes if needed
- Once approved and all checks pass, your PR can be merged!

### 🎯 Pro Tips for Success
- **Write clear commit messages** that explain what and why
- **Keep PRs focused** - one feature or fix per PR
- **Test your changes** before pushing
- **Check SonarQube results** and fix issues promptly
- **Be patient** - automated checks take a few minutes to run

### Example Complete Workflow
```bash
# 1. Start fresh
git checkout main
git pull origin main

# 2. Create feature branch
git checkout -b feature/update-contact-form

# 3. Make changes to your files
# (edit index.html, add form validation)

# 4. Stage and commit
git add .
git commit -m "Add: form validation to contact form"

# 5. Push to GitHub
git push origin feature/update-contact-form

# 6. Go to GitHub and create PR
# 7. Wait for checks, address any issues
# 8. Get approval and merge!
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

---

**Ready to start your DevSecOps journey?** Fork this repo and make your first contribution! 🚀