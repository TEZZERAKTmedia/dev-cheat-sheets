# ⚙️ GitHub Actions Cheat Sheet

## 🧪 Basic Workflow
```yaml
name: CI

on: [push, pull_request]

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3
      - name: Install dependencies
        run: npm install
      - name: Run tests
        run: npm test
```

## 🧰 Common Actions
```yaml
- uses: actions/setup-node@v3
- uses: docker/build-push-action@v5
- uses: actions/cache@v3
```

## 🔐 Secrets
```yaml
env:
  TOKEN: ${{ secrets.MY_SECRET }}
```