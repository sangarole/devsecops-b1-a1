# GitHub Actions Security Pipeline for Python

## ✅ Tools Used

| Tool       | Purpose                          |
|------------|----------------------------------|
| Bandit     | Python code linting for security |
| Gitleaks   | Detects secrets in code          |
| Trivy (FS) | Scans local code dependencies    |
| Trivy (Image) | Scans Docker image CVEs       |

## 🔧 Triggered On

- Push to `main`
- Pull Requests
- Manual runs (workflow_dispatch)

## 📊 How to Interpret Results

- **Bandit**: Shows severity of code-level issues
- **Gitleaks**: Prints found secrets with location
- **Trivy**: Lists vulnerable packages with CVE IDs and severity