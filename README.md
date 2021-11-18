# pipeline-actions

Repository with generic Github actions to cover pipeline steps for farmer connect services

## workflows

Workflows to be used within any repository. Inside a job, mention the workflow in the keyword "uses". [Instructions here](https://docs.github.com/en/enterprise-cloud@latest/actions/learn-github-actions/reusing-workflows).

### yarn-lint-build-test

Tests and builds NPM-based projects with Yarn.

### docker-build-and-push

Builds a docker image and pushes to the repository with the provided tag and as "latest".

### helm-package

Packages a Helm chart to prepare for deployment.

### aks-deploy

Deploy a Helm application to Kubernetes in AKS.

## actions

Actions are simple operations that reuse environment variables. Prefer them if the parameters for a given task are not fixed and known beforehand.

### cypress

Runs cypress tests in NPM-based projects. Requires "cypress" script in package.json with the desired command.
