# GitHub Actions Demo with Python
![Python](https://img.shields.io/badge/Python-3.x-blue.svg)
![GitHub Actions](https://img.shields.io/badge/CI%2FCD-GitHub%20Actions-yellow.svg)
![Branch Protection](https://img.shields.io/badge/Branch%20Protection-Rules-green.svg)

This project is a simple demonstration of using GitHub Actions to automate tasks in a Python project. It includes setting up branch protection rules, creating a workflow using a YAML file, testing the workflow, and configuring GitHub Secrets for environment variables.

## Features
- **Branch Protection Rules**: Ensures that certain branches, such as main, are protected and can only be modified through pull requests with passing workflows.
- **GitHub Actions Workflow**: Automates tasks such as running tests or linting the codebase whenever changes are pushed to the repository.
- **Environment Variables**: Securely manages sensitive information using GitHub Secrets.


## Setup
### Prerequisites
- Python installed locally.
- A GitHub repository to host the project.
- Basic knowledge of Git and GitHub.

### **1. Clone the Repository**
```bash
git clone https://github.com/yourusername/github-actions-demo.git
cd github-actions-demo
```

### **2. Set Up Python Environment**
Create a virtual environment and install the required packages.
```bash
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
pip install -r requirements.txt
```

### **3. Configure GitHub Actions**
**1. Create Branch Protection Rules:**

- Go to your GitHub repository.
- Navigate to Settings > Branches > Branch Protection Rules.
- Add a rule to protect the main branch.

### **2. Create Workflow:**

- In the .github/workflows directory, create a YAML file named flask_test.yml and insert the content that 
- you can find inside the file.

### **3. Test the Workflow:**

- Push changes to a new branch and open a pull request to the main branch.
- GitHub Actions will automatically run the workflow, and you should see the results on the pull request page.

## Running the Project Locally
After setting up the environment, you can run the project locally:
```bash
python app.py
```

To run tests:

```bash
python ./main_test.py
```
