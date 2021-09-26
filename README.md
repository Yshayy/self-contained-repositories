# Self contained repositories (WIP)

### Introduction

Developers today need to work very hard to understand, develop and release software.
As complexity increase, they work with multiple codebases in different programming lanugages with vast array of fragmented tools.
Git and code-based configuration can be used to control and manage these complexities and we see it already happenning in the wild with:
- Package dependencies - modern PL toolchains use configuration files to define package dependencies.
- IaC (infrastructure as code) + GitOps - Instructions for provisioning cloud infrastructure and deployment  
- Dockerfiles - self-contained instructions for building image 

Development Environments
------------------------

### Resources
- Talk: Self-contained Development Environments for everyone ([Slides](https://docs.google.com/presentation/d/1nixUW4DUCo02lJ9-zBjq4jf5B-cbZQEEzib9hR0CNUs/edit?usp=sharing)).  
  .devcontainer Code Examples (Forks):  
  - [qeesung/image2ascii](https://github.com/Yshayy/image2ascii/tree/master/.devcontainer)
  - [Habitca/Habitica](https://github.com/Yshayy/habitica/tree/develop/.devcontainer)
  - [Soluto/Tweek](https://github.com/Soluto/tweek/tree/master/.devcontainer)
  - [kubecost/cost-model](https://github.com/Yshayy/cost-model/tree/develop/.devcontainer)


### Tools & Patterns

- DevContainer

- Nested Docker

- Local kubernetes

- Mocking cloud dependencies 

- Data seeding

- Multi-Container apps

