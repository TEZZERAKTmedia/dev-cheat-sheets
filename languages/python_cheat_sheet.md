# 🐍 Python Cheat Sheet

## 🛠️ Virtual Environments
```bash
python -m venv venv
source venv/bin/activate  # Mac/Linux
venv\Scripts\activate   # Windows
deactivate
```

## 📦 Package Management
```bash
pip install package
pip freeze > requirements.txt
pip install -r requirements.txt
```

## 📜 Running Scripts
```bash
python script.py
python -i script.py  # Run and enter interactive mode
```

## 🔧 Common Libraries
```python
import os
import sys
from pathlib import Path
import json
import datetime
```

## 🧵 Async and Threads
```python
import asyncio

async def main():
    await asyncio.sleep(1)

asyncio.run(main())
```

## ✅ Testing
```bash
python -m unittest
pytest test_file.py
```

## 🐳 Dockerizing Python
```dockerfile
FROM python:3.10-slim
WORKDIR /app
COPY . .
RUN pip install -r requirements.txt
CMD ["python", "main.py"]
```