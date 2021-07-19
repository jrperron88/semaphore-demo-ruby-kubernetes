# Semaphore CI/CD demo for Kubernetes

This is an example application and CI/CD pipeline showing how to build, test and
deploy a microservice to Kubernetes using Semaphore 2.0.

Ingredients:

- Ruby Sinatra as web framework
- RSpec for tests
- Packaged in a Docker container
- Container pushed to Docker Hub registry
- Deployed to Kubernetes

## Improvements to be made
 - Move configuration to environment variables (region,ECS uri)
 - Develop a system to not use latest with each image to aid with rollback strategy
 - Develop a rollback strategy
 - Use IaC for EKS instead of relying on eksctl for deployment
 - Configure EKS cluster to scale with traffic

## License

Copyright (c) 2019 Rendered Text

Distributed under the MIT License. See the file LICENSE.
