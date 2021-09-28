# Self contained repositories (WIP)

### Introduction

Developers today need to work very hard to understand, develop and release software.
As complexity increase, they work with multiple codebases in different programming lanugages with vast array of fragmented tools.
Git and code-based configuration can be used to control and manage these complexities and we see it already happenning in the wild with:
- Package dependencies - modern PL toolchains use configuration files to define package dependencies.
- IaC (infrastructure as code) + GitOps - Instructions for provisioning cloud infrastructure and deployment  
- Dockerfiles - self-contained instructions for building image 

Taking it further, a "self-contained" repository can contain futher configurations to include (but not limited to):
- Documentation sites
- Development environment configuration
- CI Pipeline defintions
- Encrypted secrets
- Security poilicies
- API defintions
- And more....

By making all these defintions contained in our source control,we can better developer experience and lower the barrier for developing, building and depolying complex applications at any revsion.

This document designed to document and aggregate tools & practices that can be used to make repositories self-contained.

### Status

This is a living document, currently at a very early stage.
PRs and tool suggestions and improvement are most welcome.  

  
# Principles

## Development Environments


This section should focus on how we can define our development environment configuration in our repository in order to enable the creation of development enviroments that are tailored to our project.

### Resources
----------

- Talk: Self-contained Development Environments for everyone ([Slides](https://docs.google.com/presentation/d/1nixUW4DUCo02lJ9-zBjq4jf5B-cbZQEEzib9hR0CNUs/edit?usp=sharing)).  
  .devcontainer Code Examples (Forks):  
  - [qeesung/image2ascii](https://github.com/Yshayy/image2ascii/tree/master/.devcontainer)
  - [Habitca/Habitica](https://github.com/Yshayy/habitica/tree/develop/.devcontainer)
  - [Soluto/Tweek](https://github.com/Soluto/tweek/tree/master/.devcontainer)
  - [kubecost/cost-model](https://github.com/Yshayy/cost-model/tree/develop/.devcontainer)


### Tools & Patterns
-----------

**DevContainer**

  Developing inside a container instead of directly on machine.
  In the container we can define all the SDKs, CLIs, programming languges runtime, tools, extendsions and other dependencies.
  
  Using VS Code:  
  - Install [Code Remote containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers) extension
  - Try opening a project in a development container
  - Customize your Dockerfile in devcontainer.json

  Examples:
  - [VSCode dev containers repository](https://github.com/microsoft/vscode-dev-containers/tree/main/containers)

**Nested Docker**

**Local kubernetes**

**Mocking cloud dependencies**

**Data seeding**

**Multi-Container apps**

