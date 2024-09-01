# GitHub Actions

GitHub Actions is a continuous integration and continuous delivery (CI/CD) platform that allows you to **automate** your build, test, and deployment pipeline

## Introduction

- GitHub Actions is a **CI/CD pipeline directly integrated with github repository**

- It allows us to **automate**:

  - Running Test Suits
  - Building Images
  - Compiling static sites
  - Deploying code to servers

- GitHub Actions files are defined as **YAML** files located in the _.github/workflow_ folder in the repo.

- GitHub Actions has **templates** that one can use.

- Can have multiple **workflows** in repo triggered by different events.

## Components

- GitHub Actions workflows can be **triggered by events** in a repository, such as a pull request or an issue being created.
- A workflow consists of one or more **jobs**.
- Jobs can run _sequentially_ or in _parallel_.
- Each job runs in its own **virtual machine runner** or a container.
- Jobs contain steps that either:
  - Run a **script** defined by the user.
  - Run an **action**, which is a reusable extension to simplify the workflow.

## References

- [GitHub Docs](https://docs.github.com/en/actions/about-github-actions/understanding-github-actions)

- [Exam Pro](https://www.exampro.co/github-actions)

- [Microsoft Learn](https://learn.microsoft.com/en-us/training/modules/github-actions-automate-tasks/?source=docs)
