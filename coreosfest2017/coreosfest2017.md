# CoreOS Fest 2017

## Introduction

CoreOS Fest 2017 was held May 31 - June 1, 2017 in at Pier 27 in San Francisco, CA.  The full conference schedule
including recording of sessions is [posted online](https://coreos.com/fest/#schedule).

## Keynote: Alex Polvi, CoreOS CEO

1. Techtonic
  * Automated administration

1. etcd as a Service
  * Cloud service agnostic
  * Managed backups
  * high uptime

## Azure Announcement
[Draft](https://github.com/Azure/draft): Streamlined Kubernetes Development
  * Draft makes it easy to build applications that run on Kubernetes. Draft targets the "inner loop" of a developer's workflow: as they hack on code, but before code is committed to version control.
  * 100% Open Source
  * Eases a developers container development path
  * Builds a container and schedules it in a k8s cluster

   ```
   draft create
   docker up
   ```

  * Draft Packs (6 pack)
    * python
    * ruby
    * node
    * golang
    * #5
    * #6


## Kubernetes and GCP

### GKE

1. Resiliant
1. High Performance & Low Cost

Personally, I keep on hearing that GCP has made great strides in 2016 & 2017 and is the Cloud proider to move to.


### Brief History

  * Borg -> Omenga -> Kubernetes
  * Kubernetes is much more flexible and customizeable
  * Kubernetes


## Writing a custom Controller: Extending the functionality of Controlers

Aaron Levy, CoreOS

### What is a controller?

A custom controller takes your cluster towards a desired state.

### CoreOS Operators

1. Coodinating Container Linux updates across nodes
1. etcd-operator

### Example: Node Reboot Operator

Example: https://github.com/aaronlevy/kube-controller-demo

Other Resources to investigate when writing a controller:

* Shared Informers
* Events


## Federated clusters

Dan Wilson, Concur
k8s @ concur

Why Kubernetes
* Extensible API

Why CoreOs?
* Simple updates by channel
* Designed to run in a cluster

https://github.com/concur/kubegowatcher

### Deployment Approaches

1. use kubctl and apply on individual projects
1. k8s spec repo
  * Job to pull and process the spec Repo
  * `kubectl apply`
1. Custome Pipeline
  * Build into the CI/CD system
  * Run `kubectl` or make API call
1. Write custom tooling using the API

### Setting up k8s Federation

Disclaimer: k8s federation is an _alpha_ feature
* https://kubernetes.io/docs/concepts/cluster-administration/federation/
* https://github.com/kelseyhightower/kubernetes-cluster-federation

[Skipper](https://github.com/concur/skipper)
  *  a tool to command your fleet of k8s clusters

### Federation Options
  * Cluster Selectors
  * Cluster Tainting

## Kubernetes Networking

Overview of flannel, calico and canal.

Highlights:
* Canal is simply
* Calico ingresses

## Day 2 Keynote

1. [CNI: Container Networking Interface](https://github.com/containernetworking/cni)
  * Weave
  * flannel
  * calico
  * canal
1. rkt: v1.26 releases
1. Prometheus
  * v2.0: Improved Storage Engine and remote storage API
  * Less memory
  * less i/o
1. Clair 2.0: Static Container Image Analysis
  * CoreOS open source project for the static analysis of vulnerabilities in application containers (currently including appc and docker).

### Kubernetes: State of the Union

1. Releasing High Quality k8s
  * High community involvement!
  * ~3mo development cycle
  * ~9mo patch cycle
  * Blameless postmortems

## Cloud Native and the Rise of the Streamlined
Chris Jones, SRE @ Google

What is Site Reliability Engineering (SRE)?
* Google wrote the book on SRE.  Literally!
   * Read Online: g.co/srebook
* Keep software systems running
* Monitoring is at the core of what SREs do

Software: In Operations
* Monitoring
* Data Integrity
* Capacity Planning
* Configuration Management
* Deployment Automation
* Automated Repair
