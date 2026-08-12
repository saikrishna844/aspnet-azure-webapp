# Azure ASP.NET Portfolio with Secure CI/CD

[![Build and Deploy](https://github.com/saikrishna844/aspnet-azure-webapp/actions/workflows/main_saikrishna-aspnet-cicd-2026.yml/badge.svg)](https://github.com/saikrishna844/aspnet-azure-webapp/actions/workflows/main_saikrishna-aspnet-cicd-2026.yml)

A professional ASP.NET Core portfolio automatically built and deployed to Azure App Service using GitHub Actions and secure OpenID Connect authentication.

## Live Website

[View the live Azure portfolio](https://saikrishna-aspnet-cicd-2026-gccnf0ckexd8gjfy.centralindia-01.azurewebsites.net)

## Project Overview

This project demonstrates a complete cloud application delivery workflow:

- Developed a responsive portfolio using ASP.NET Core Razor Pages
- Stored and version-controlled the application in GitHub
- Implemented continuous integration and deployment using GitHub Actions
- Configured secretless Azure authentication using OpenID Connect
- Built and packaged the application automatically
- Deployed the generated artifact to Azure App Service
- Hosted the project cost-effectively using the Azure F1 Free tier

## Architecture

```mermaid
flowchart TD
    A[Developer] -->|Git push| B[GitHub Repository]
    B --> C[GitHub Actions]
    C --> D[Restore and Build]
    D --> E[Deployment Artifact]
    E --> F[OIDC Authentication]
    F --> G[Azure Managed Identity]
    G --> H[Azure App Service]
    H --> I[Live Portfolio Website]
