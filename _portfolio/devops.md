---
title: "CRUD API DevOps pipeline"
excerpt: "A complete CI/CD pipeline for a Spring Boot REST API, with automated testing and security scanning, container releases and IaC deployment, built with GitHub Actions, Docker and Terraform.<br/><img src='/images/devops.png'>"
collection: portfolio
date: 2026-02-01
---

This project was built around a small Spring Boot CRUD API service in Java. The main focus was a complete, automated continuous delivery pipeline on GitHub.

On every push and pull request, GitHub Actions runs parallel jobs: a style check with Checkstyle, a Maven build with unit and integration tests, a Trivy scan for vulnerable dependencies, exposed secrets and misconfigurations, and a Docker job that builds the image, scans it and runs a smoke test against the application's health check. Pushing a version tag starts a separate release workflow, which publishes the container image to the GitHub Container Registry, generates a CycloneDX software bill of materials and attaches it to a new GitHub release.

The release is then deployed automatically. Terraform with the Multipass provider creates an Ubuntu virtual machine, installs Docker through cloud-init and starts the container, and a final step verifies that the service responds. We split the pipeline into three workflows with their own triggers and permissions, with the self-hosted runner protected by branch protection rules.

The project gave me pratical experience designing automated DevOps pipelines and balancing speed, security and reproducibility in the process.

View the [repository](https://github.com/eryngia/dd2482-project).

![DevOps](/images/devops.png)