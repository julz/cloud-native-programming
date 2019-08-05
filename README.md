# A Cloud Native Programming Manifesto

## Values

1. _Consistency_ over configuration -- that is, where possible we prefer to focus on code, not CRDs or yml or ReplicaSets or helm charts or Dockerfiles. 12-factor apps and serverless functions can help with this.
1. _Monoliths_ over micro-services -- that is, where possible we resist breaking down a system in to more micro-services than required (generally, a service per team is a good rule-of-thumb)
1. _Routing_ over deployment -- rather than managing multiple environments, where possible we prefer progressive deployment, observability and feature flags
1. _Services_ over managing state -- that is, we prefer to use existing services at the highest level of abstraction possible rather than managing databases and complex systems

## Resources:

PaaS:

- [Cloud Foundry](https://cloudfoundry.org) - A popular PaaS for 12-factor apps
- [Knative](https://knative.dev) - Kubernetes-native CRDs for 12-factor apps and functions

Code-to-container:

- [Cloud Native Buildpacks](https://buildpacks.io) - Abstracts the details of building and updating containers from code
- [Tekton](http://tekton.dev) - Kubernetes-native pipeline CRDs, useful for building code-to-container pipelines
