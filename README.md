# Docker Web App

A lightweight containerized web application demonstrating Docker fundamentals with nginx and interactive frontend.

## Overview

Simple yet complete Docker project showcasing:
- Container orchestration with nginx:alpine
- Static file serving in production environment  
- Port mapping and container lifecycle management

## Quick Start

```bash
# Build and run
docker build -t my-webapp .
docker run -d -p 8080:80 my-webapp 
```

**Access:** http://localhost:8080

## Project Structure

```
├── Dockerfile    
├── index.html       
├── style.css       
└── script.js       
```

## Technical Stack

- **Base Image:** nginx:alpine (lightweight, production-ready)
- **Frontend:** HTML5, CSS3, JavaScript
- **Container:** Docker with port mapping (80 → 8080)

## Requirements

- Docker Desktop or Docker Engine
- Modern web browser

## Common Issues & Solutions

**Build Context Missing**
```bash
# Error: requires 1 argument
# Solution: Add build context
docker build -t webapp .  # ← Don't forget the dot
```

**Dockerfile Not Found**
```bash
# Error: no such file or directory
# Solution: Ensure exact filename (no extension)
```

**WSL Backend Issues**
```bash
# Error: Docker Desktop requires WSL 2
# Solution: Update WSL to latest version
wsl --update
# Restart required after WSL update
```

**Docker Command Not Found**
```bash
# Error: 'docker' is not recognized
# Solution: Install Docker Desktop for Windows
# Verify: docker --version
```

---

**Learning Focus:** Docker containerization, image building, and deployment fundamentals.

---

**Final results**
<img width="1911" height="1028" alt="image" src="https://github.com/user-attachments/assets/b14ff47d-18db-4290-a9bd-6d2e6981dc3f" />

