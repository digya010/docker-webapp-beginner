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
├── Dockerfile      # nginx:alpine configuration
├── index.html      # Application frontend  
├── style.css       # Responsive styling
└── script.js       # Interactive features
```

## Docker Commands

```bash
# Background mode
docker run -d -p 8080:80 --name webapp-container webapp

# Container management  
docker ps                 # List running containers
docker logs webapp-container   # View logs
docker stop webapp-container   # Stop container
```

## Technical Stack

- **Base Image:** nginx:alpine (lightweight, production-ready)
- **Frontend:** HTML5, CSS3, Vanilla JavaScript
- **Container:** Docker with port mapping (80 → 8080)

## Requirements

- Docker Desktop or Docker Engine
- Modern web browser

---

**Learning Focus:** Docker containerization, image building, and deployment fundamentals.
