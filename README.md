# Technical Documentation

<!-- Main themes -->
### [Architecture](architecture/README.md)
### [Development workflow](development_workflow.md)

<!-- mostly helpers and stimulus controllers -->
## Components
### [Select](components/select.md)
### [Dropdown](components/dropdown.md)

## API Documentation

The documentation URL: https://awesome.infinum.co/api/v1/docs/

## Deployment
here is some new line
[Semaphore](https://semaphoreci.com/rails-awesome)

### Builds
Our continuous integration tool will automatically build the environment upon each push to whatever branch.
The build installs all dependencies and runs all the specs.

### Deploying
The `staging` branch is used for the staging environment and `master` for production.
Whenever a branch or pull request is merged to one of those environments, after the build is finished Semaphore will try to deploy it to the environment.
