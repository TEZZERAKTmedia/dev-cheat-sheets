# 🧠 Dev Cheatsheets Collection

This repository is a curated collection of fast-access, practical cheat sheets for daily development use. It includes everything from beginner-friendly command references to advanced DevOps workflows, embedded systems tooling, and AR/VR development techniques.

Even the simplest commands are included intentionally — to save time, reduce cognitive load during deep-focus work, and act as a reliable daily reference.

---

## 📂 Categories

Organized into folders by domain:

- [Git](./git) – commits, branches, merge strategies, and common workflows
- [Docker](./docker) – build/run syntax, container cleanup, and Compose usage
- [GitHub](./github) – Actions, PR tips, repo permissions, security
- [Languages](./languages) – Python, JS, C/C++, Bash snippets, and more
- [Makefile](./makefile) – common recipes, conditional blocks, CLI flags
- [Embedded](./embedded) – serial protocols, memory-safe patterns, GPIO commands
- [AR/VR](./ar-vr) – Unity XR, ARKit/ARCore setup, Barracuda, object detection
- [VM Setup](./vm) – for running full Linux workflows on macOS (see below)

---

## 💻 macOS Kernel Limitation & Linux VM Workaround

Some cheat sheets reference tools that simulate hardware behavior using `socat` and Linux device interfaces like `/dev/ttyS0`. These are **not compatible with macOS**, since Docker on macOS runs inside a lightweight virtual machine without native PTY access or full `/dev` mapping.

To overcome this, the `vm/` section provides a full guide to setting up an **Ubuntu VM via Multipass**. This gives you access to a real Linux kernel and allows Docker and `socat` to simulate serial devices properly — ideal for embedded systems development or testing workflows that rely on low-level device access.

---

## ✅ Goal

This repo exists to serve as a trusted go-to reference — no fluff, just clean, useful knowledge for working developers across platforms and domains.

Feel free to clone, fork, and customize for your own stack.

