# Metadata

* Attributes, Labels, and Tags
* Frozen vs. Wandering
* Non-unique vs. Context-unique
* Builds, Releases, and Stages
* Versioning
* Metadata Repositories
* Auomated Governance of Metadata


# Templating

* Web vs. Non-Web
* Burden of Runtimes
* Burden of Polyglot
* The Non-Twelve Factor App: Configuration on Disk
* Template Repositories


# Secrets

* Ramdisks
* Metadata
* Data at rest / in-motion
* Decrypt long TTL key, re-encrypt short TTL key
* Reln with Templating
* Secret Repositories
* AWS SSM Parameter Store vs. Hashicorp Vault vs. Spring Cloud Config Server
* Large Secrets (PEMs)
* AuthZ: AppDev/Quality vs. Operators vs. Automation. Environments. RBAC


# Building & Packaging

* Synching Central Repositories with Cluster Repositories
* Secrets for Builders
* Containers are your built bytes and static assets
* Containers do _not_ have your templated configuration or secrets
* Build runs and metadata


# Deployment

* _The Who_ and _The Where_
* Environments vs. Stages. No Superenvironment, subenvironment, "Stage", or "Staging"
* Reln with Stage-based Metadata
* Materializing with template invocations, intermingled with secrets
* Deployments are transient
* Deployments do not store (long-term)
* Builders are deployments, too. (Don't store, don't coddle as pet)


# Think Local

* Storage API. S3 vs. Minio
* Parameter API.
* Docker Swarm


# Development

* Dockerfiles should be _The What_ and a little of _The Who_. Redirect _The How_ to COPY'd scripts
* No dashes in group names or project names
* High-level infrastructure layout versioned in the project
* Dockerfiles and Compose files versioned in the project
* Jenkinsfiles versioned in the project
* Runtimeless: go-lang and crystal-lang
* You cannot escape Bash


# Tracing

* TBD


# Streaming

* Multi-source, multi-destination queue configuration by fixed aliases
* Tracing
* Centralized Logging & Metrics


# Tooling

* Jenkisfiles have _waaay_ too much of _The How_
