  # GitHub Actions Lab
**Student Name:** Rutvi Panchal

**Student ID:** 991755961

## Purpose of Workflow 1

The Dependent Jobs Workflow demonstrates job dependencies using the `needs` keyword. The workflow executes jobs in the following order:

Build → Test → Deploy

This ensures that testing only occurs after a successful build, and deployment only occurs after successful testing.

## Purpose of Workflow 2

The Multi Platform Workflow demonstrates parallel execution across multiple operating systems.

The workflow runs simultaneously on:

* Ubuntu
* Windows
* macOS

This helps verify that the project behaves correctly on different platforms.

## Key Concepts Demonstrated

### needs

Creates dependencies between jobs and controls execution order.

### runs-on

Specifies the operating system used to run a job.

### Actions

Uses `actions/checkout@v4` to download repository code into the runner environment.

## Challenges Faced

One challenge was correctly configuring GitHub Actions workflow syntax, especially ensuring proper indentation and defining the on trigger correctly. This was resolved by carefully reviewing YAML structure and validating the workflow file before pushing.

Another challenge was understanding how to manage workflow execution across multiple operating systems. This was resolved by using OS-specific commands and testing each job separately in the GitHub Actions environment.
