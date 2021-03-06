# pipeline-actions

Repository with generic GitHub actions to cover pipeline steps for farmer connect services.

## Workflows

Workflows to be used within any repository. Inside a job, mention the workflow in the keyword "uses". [Instructions here](https://docs.github.com/en/enterprise-cloud@latest/actions/learn-github-actions/reusing-workflows).

### yarn-lint-build-test

Tests and builds NPM-based projects with Yarn.

### docker-build-and-push

Builds a docker image and pushes to the repository with the provided tag and as "latest".

### helm-package

Packages a Helm chart to prepare for deployment.

### aks-deploy

Deploys a Helm application to Kubernetes in AKS.

### apply-db-migration

Generates and applies a DB migration with Entity Framework.

## Actions

Actions are simple operations that reuse environment variables. Prefer them if the parameters for a given task are not fixed and known beforehand.

### cypress

Runs cypress tests in NPM-based projects. Requires "cypress" script in package.json with the desired command.

### dotnet-5-test

Tests and builds .NET-based projects in version 5.

### dotnet-6-test

Tests and builds .NET-based projects in version 6.
