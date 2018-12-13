# Eleventy Static Site Generator Test

This repo is my attempt to test out Azure Pipelines to build static content from pull requests.

---

[![Build Status](https://dev.azure.com/marcmodin/pipelines.eleventy-shortcomps/_apis/build/status/marcmodin.pipelines.eleventy-shortcomps?branchName=build)](https://dev.azure.com/marcmodin/pipelines.eleventy-shortcomps/_build/latest?definitionId=3?branchName=build)

## Cloned from eleventy-shortcomps

Eleventy-Shortcomps Starter project for static site, using [Eleventy](https://11ty.io) and shortcode components (AKA _shortcomps_) pattern.

## Steps Taken

1. create a pipeline project on Azure Devops [Azure Devops](https://azure.microsoft.com/en-us/services/devops/)

2. Configure Azure Pipelines to use your Git repo. [Get Started](https://docs.microsoft.com/en-us/azure/devops/pipelines/get-started-yaml?view=vsts)

3. Follow the wizard to commit the YAML config file to your repo

4. Create your build project or clone this repo locally

## Git Workflow

I use the following git workflow to push changes and automatically build and push the created content to `docs` folder on the master branch.

- Always branch off the build-branch
- Push the feature-branch commits
- Create pull-requests to the build-branch
- This fires off the Pipeline Build which pushes the generated docs back onto the build-branch
- Merge and Delete feature-branch
- Create a pull-request from build-branch to the master-branch
- Merge commits

## Further Steps

**Currently working on this README**

Feedback welcome 🙌
