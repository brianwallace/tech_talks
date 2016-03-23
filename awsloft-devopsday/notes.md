# AWS Dev Ops Days

# Intro Talk

## What is DevOps?

"Anything that results in increased development efficiency"

- Full ownership
  - Designing services
  - Implementing services
  - writing tests
  - Operating services in production
- Full accountability
- Aligned incentives

### Core Values

Culture
- ownership
- accountability

Operations
- Automate all changes
- Deploy often and monitor everything

Process
- Weekly metric reviews
  - Grow good metrics
  - Hunt down bad anomalies and squash the root cause
- Bar raisers

## Monolithic App

build > test > release

Once a critical mass of developers is reached, integration becomes painful.

component1: developers -> -> build > test > release
component2: developers -> -> build > test > release
component3: developers -> -> build > test > release

## Tools development

### Tools Development Philosophy
* Self-service
* Bake best practices into the tools themselves
* Technology agnostic
* Single-purpose services

### Key Tools
1. Code Deploy
1. Code Pipeline


## AWS Code services

1. Code Deploy (Apollo)
1. Code Pipeline
1. Code Commit


# Consul and Code Deploy

* Service Health Checks
* Orchestrate Deployments
* Application Configuration
* Maintenance Mode for Nodes
