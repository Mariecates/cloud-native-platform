cloud-native-platform

A cloud-native application built with Node.js and Express, designed to demonstrate practical DevOps, Cloud, Infrastructure as Code, CI/CD, containerization, security, observability, and platform engineering skills.

This project starts with a simple Express application and progressively evolves into a production-oriented cloud-native platform.

The goal is not just to build an application, but to demonstrate how modern applications are built, tested, packaged, deployed, monitored, and operated in the cloud.

Project Goals

This repository is designed to demonstrate middle-to-senior-level skills across:

Cloud infrastructure

DevOps automation

CI/CD pipelines

Docker and containerization

Infrastructure as Code

Kubernetes

Cloud networking

Application security

Secrets management

Monitoring and observability

Logging

Automated testing

Deployment strategies

Infrastructure automation

Reliability and scalability

Current Version
Version 1 — Express Application

The current version establishes the application foundation using Node.js and Express.

At this stage, the project demonstrates:

Express application setup

HTTP fundamentals

Express routing

Static file serving

Node.js package management

Local development

Basic troubleshooting

Git-based source control

Future versions will progressively introduce DevOps and cloud engineering capabilities.

Technology Roadmap

The project will evolve through multiple stages:

Express Application
        │
        ▼
Docker Containerization
        │
        ▼
Automated Testing
        │
        ▼
CI Pipeline
        │
        ▼
Security Scanning
        │
        ▼
Infrastructure as Code
        │
        ▼
Cloud Infrastructure
        │
        ▼
Kubernetes
        │
        ▼
Continuous Deployment
        │
        ▼
Observability
        │
        ▼
Production-Ready Platform

Architecture Evolution

The initial architecture is intentionally simple:

              ┌─────────────────┐
              │     Browser     │
              └────────┬────────┘
                       │
                       ▼
              ┌─────────────────┐
              │  Express App    │
              │    Node.js      │
              └────────┬────────┘
                       │
                       ▼
              ┌─────────────────┐
              │ Static Content  │
              │    /public      │
              └─────────────────┘


As the project evolves, the architecture will move toward:

                         ┌──────────────────┐
                         │      Users       │
                         └────────┬─────────┘
                                  │
                                  ▼
                         ┌──────────────────┐
                         │ Load Balancer /  │
                         │    Ingress       │
                         └────────┬─────────┘
                                  │
                                  ▼
                    ┌──────────────────────────┐
                    │       Kubernetes         │
                    │                          │
                    │  ┌────────────────────┐  │
                    │  │   Express App      │  │
                    │  │    Containers      │  │
                    │  └────────────────────┘  │
                    │                          │
                    └───────────┬──────────────┘
                                │
                ┌───────────────┼────────────────┐
                ▼               ▼                ▼
           Monitoring        Logging         Cloud Services

Current Project Structure
cloud-native-platform/
├── public/
│   └── index.html
├── index.js
├── package.json
├── package-lock.json
└── README.md


The structure will expand as infrastructure and automation are introduced.

Requirements

Before running the application locally, install:

Tool	Purpose
Node.js	JavaScript runtime
npm	Package management
Git	Source control
VS Code	Recommended development environment
Terminal	Command-line operations
Running the Application Locally
1. Clone the repository
git clone <repository-url>
cd cloud-native-platform

2. Install dependencies
npm install

3. Start the application
node index.js


You should see:

Server is running at http://localhost:3000

4. Open the application

Navigate to:

http://localhost:3000

Application Configuration

The application currently runs on port 3000.

A future version will use environment variables for configuration, for example:

PORT=3000
NODE_ENV=development


This will allow configuration to be separated from application code as the project moves toward containerized and cloud deployments.

Example Express Route

The application can be extended with additional routes:

app.get('/about', (req, res) => {
  res.send('About this application');
});

DevOps Engineering Roadmap

The project will be developed incrementally.

Phase 1 — Application Foundation

Node.js

Express

HTTP

Routing

Static content

Git

Status: 🟢 In Progress

Phase 2 — Containerization

Docker

Dockerfile

Docker Compose

Container networking

Image optimization

Multi-stage builds

Status: 🔵 Planned

Phase 3 — CI/CD

GitHub Actions

Automated testing

Build pipelines

Container image builds

Artifact management

Deployment automation

Status: 🔵 Planned

Phase 4 — Security

Dependency scanning

Container image scanning

Secret management

Least-privilege principles

SAST

Supply-chain security

Status: 🔵 Planned

Phase 5 — Infrastructure as Code

Terraform

Cloud networking

IAM

Compute resources

Storage

Infrastructure modules

Remote state management

Status: 🔵 Planned

Phase 6 — Kubernetes

Kubernetes fundamentals

Deployments

Services

ConfigMaps

Secrets

Ingress

Health checks

Resource requests and limits

Horizontal Pod Autoscaling

Status: 🔵 Planned

Phase 7 — Observability

Metrics

Logging

Distributed tracing

Application health checks

Dashboards

Alerting

SLO/SLI concepts

Status: 🔵 Planned

Phase 8 — Production Engineering

High availability

Scalability

Disaster recovery

Rolling deployments

Blue/green deployments

Canary releases

Backup and recovery

Cost optimization

Status: 🔵 Planned

Skills Demonstrated

The completed project is intended to demonstrate practical experience with:

Cloud Engineering
├── AWS / Azure / GCP
├── Networking
├── IAM
└── Cloud Security

DevOps
├── Git
├── GitHub Actions
├── CI/CD
├── Automation
└── Release Management

Containers
├── Docker
├── Docker Compose
└── Container Security

Infrastructure as Code
├── Terraform
├── Modules
├── State Management
└── Infrastructure Automation

Kubernetes
├── Deployments
├── Services
├── Ingress
├── Secrets
├── ConfigMaps
└── Autoscaling

Observability
├── Metrics
├── Logs
├── Traces
├── Dashboards
└── Alerting

Security
├── SAST
├── Dependency Scanning
├── Container Scanning
├── Secrets Management
└── Least Privilege

Development Philosophy

This project follows several engineering principles:

Automation over manual processes

Infrastructure as Code

Security by design

Immutable infrastructure

Reproducible environments

Version-controlled infrastructure

Continuous integration and delivery

Observability-driven operations

Least privilege

Documentation as code

Troubleshooting
node: command not found

Install Node.js and restart your terminal.

Port 3000 is already in use

Identify the process using port 3000 or change the application port.

Application is not loading

Verify that the server is running:

node index.js


Then visit:

http://localhost:3000

Future Improvements

Planned improvements include:

 Add automated unit tests

 Add Dockerfile

 Add Docker Compose

 Add GitHub Actions CI pipeline

 Add linting and code quality checks

 Add dependency vulnerability scanning

 Add container security scanning

 Add Terraform infrastructure

 Deploy infrastructure to the cloud

 Deploy application to Kubernetes

 Add Helm

 Add monitoring

 Add centralized logging

 Add alerting

 Implement production deployment strategies

 Document architecture decisions

Project Objective

The long-term objective of cloud-native-platform is to demonstrate the complete lifecycle of a modern cloud-native application:

Plan
  ↓
Code
  ↓
Build
  ↓
Test
  ↓
Secure
  ↓
Package
  ↓
Provision
  ↓
Deploy
  ↓
Monitor
  ↓
Improve


This repository is intended to serve as a practical demonstration of DevOps and Cloud Engineering capabilities from application development through production operations.

Author

Marie

© 2026 Marie
