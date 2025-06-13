# 🔀 Git + Docker Combined Cheat Sheet

## 🧪 Common Workflows

### 🔧 Clone and Build Docker Image
```bash
git clone https://github.com/username/repo.git
cd repo
docker build -t repo-image .
docker run -p 3000:3000 repo-image
```

### 🚀 Tag Docker Image with Git Commit SHA
```bash
docker build -t my-app:$(git rev-parse --short HEAD) .
docker run my-app:$(git rev-parse --short HEAD)
```

### 🔁 Mount Git Repo into Docker for Dev
```bash
docker run -v $(pwd):/app -w /app node:18 bash
```

### 🔐 Use Git in CI/CD Docker Pipelines
```yaml
# GitHub Actions
steps:
  - uses: actions/checkout@v3
  - run: |
      docker build -t my-app:${{ github.sha }} .
      docker push my-app:${{ github.sha }}
```

---

## 🛠️ Troubleshooting

- `fatal: not a git repository`: Ensure volume mount or Dockerfile has `.git`
- `permission denied`: Use proper `USER` in Dockerfile