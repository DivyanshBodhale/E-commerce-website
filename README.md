# ecommerce-website

The pipeline ensures:

Code quality verification
Security vulnerability detection
Dependency scanning
Container image creation
Automated build and deployment workflow

The objective is to shift security left by integrating security checks early in the development lifecycle.

| Technology                  | Purpose                |
| --------------------------- | ---------------------- |
| **HTML / CSS / JavaScript** | Frontend Development   |
| **Git & GitHub**            | Version Control        |
| **GitHub Actions**          | CI/CD Pipeline         |
| **Docker**                  | Containerization       |
| **Trivy / Security Tools**  | Vulnerability Scanning |
| **HTMLHint**                | Code Linting           |
| **Node.js**                 | Tool Installation      |


Developer Push → GitHub Repository
        ↓
GitHub Actions Pipeline
        ↓
Code Quality Checks (Linter)
        ↓
Secrets Detection
        ↓
Dependency Vulnerability Scan
        ↓
Docker Image Build
        ↓
Container Security Scan
        ↓
Push Image to DockerHub


# Features

✔ Automated CI/CD pipeline using GitHub Actions
✔ Code linting for quality checks
✔ Secrets scanning to prevent credential leaks
✔ Dependency vulnerability scanning
✔ Docker image build automation
✔ Container security scanning
✔ Secure DevSecOps workflow


DevSecOps-Ecommerce/
│
├── .github/
│   └── workflows/
│        ├── code-quality.yml
│        ├── secrets-scan.yml
│        ├── dependency-scan.yml
│        ├── docker-scan.yml
│        └── pipeline.yml
│
├── src/
│   ├── index.html
│   ├── styles.css
│   └── script.js
│
├── Dockerfile
├── README.md
└── package.json

Pipeline Stages

1️⃣ Code Quality Check

Uses HTMLHint
Ensures code follows best practices

2️⃣ Secrets Scan
Detects exposed API keys or credentials

3️⃣ Dependency Scan
Identifies vulnerabilities in project dependencies

4️⃣ Docker Build
Builds Docker container for the application

5️⃣ Container Security Scan
Uses Trivy to scan Docker images for vulnerabilities

6️⃣ Push to DockerHub
Securely pushes the image using GitHub secrets

