# 🛠️ Common Makefile Patterns

## 🎯 Basic Structure
```make
.PHONY: build run clean

build:
	docker build -t my-app .

run:
	docker run -p 3000:3000 my-app

clean:
	docker system prune -f
```

## 🧪 Useful Patterns
```make
SHELL := /bin/bash
VERSION := $(shell git rev-parse --short HEAD)

tag:
	docker build -t my-app:$(VERSION) .
```

## 📂 Tips
- Use tabs (not spaces)
- `.PHONY` prevents conflicts with file names
- Variables make targets reusable