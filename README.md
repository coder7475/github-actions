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

### Events

- An event is a specific activity in a repository that triggers a workflow run.

- Examples include creating a pull request, opening an issue, or pushing a commit. Workflows can also be triggered on a schedule, via a REST API, or manually.

### Jobs

- A job is a set of steps in a workflow executed on the same runner.

  - Each step can either be a shell script or an action.

  - Steps are executed sequentially and can share data between them since they run on the same runner.

- Jobs can be configured to run independently or have dependencies on other jobs. By default, jobs run in parallel unless a dependency is specified.

- For example, multiple build jobs can run in parallel, and a packaging job can depend on their successful completion.

### Actions

- An action is a reusable application for the GitHub Actions platform that performs complex but repetitive tasks.

- Actions help reduce repetitive code in workflows, such as setting up the build environment or authentication.

- You can create custom actions or use actions available in the GitHub Marketplace.

### Runners

- A runner is a server that executes workflows when triggered.

- Each runner runs a single job at a time.

- GitHub provides runners for Ubuntu Linux, Microsoft Windows, and macOS, each running on a newly provisioned virtual machine.

- GitHub also offers larger runners for more demanding workloads.

- Alternatively, you can host your own runners for custom operating systems or specific hardware needs.

## References

- [GitHub Docs](https://docs.github.com/en/actions/about-github-actions/understanding-github-actions)

- [Exam Pro](https://www.exampro.co/github-actions)

- [Microsoft Learn](https://learn.microsoft.com/en-us/training/modules/github-actions-automate-tasks/?source=docs)
