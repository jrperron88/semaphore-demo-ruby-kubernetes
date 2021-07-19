# Semaphore CI/CD demo for Kubernetes

This is an example application and CI/CD pipeline showing how to build, test and
deploy a microservice to Kubernetes using Semaphore 2.0.

Ingredients:

- Ruby Sinatra as web framework
- RSpec for tests
- Packaged in a Docker container
- Container pushed to ECS
- Deployed to EKS

## Choice in Technologies
 - Wanted to use this exercise as a learning experience - used a guide to get started.
 - Most experience is in Azure Pipelines or TravisCI for CI/CD and Azure Kubernetes Service for k8s.
 - Semaphore was free to use and provided the needed CI/CI functionality.

## Improvements to be made
 - Move configuration to environment variables (region,ECS uri)
 - Develop a system to not use latest with each image to aid with rollback strategy
 - Develop a rollback strategy
 - Use IaC for EKS instead of relying on eksctl for deployment
 - Configure EKS cluster to scale with traffic

## License

Copyright (c) 2019 Rendered Text

Distributed under the MIT License. See the file LICENSE.
