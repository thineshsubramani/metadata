# Metadata

This repo holds all the metadata that I needed for my all projects, servers etc.
It helps me centrally manage configurations for all my systems with single source of truth, complete with versioning in sub-directories similar to how APIs are structured.
I like to keep things organized, scalable, and future-proof.

## Purpose

* Centralized config management across different OS and environments
* Built-in versioning to track config changes over time
* Acts as a single source of truth for my automation and sync tools

## Contains

Primarily text-based configuration files:

* `.ini`, `.env`, `.json`, `.yaml` formats

## Structure

Configurations are grouped in a clean directory hierarchy:

```
ubuntu/v1/         # Configs specific to Ubuntu systems
centos/v1/         # Configs specific to CentOS systems
init/v1/           # Configs used to bootstrap new VMs/servers
toolbox/v1/        # Configs to set up my personal toolchain and utilities
repositories/v1/   # Configs for syncing and pulling repositories
```

## Special Sub-dirs [Require client Side logics to support this]
These sub-directories inherit and extend configs from their parent; they can also override if there’s a name clash.
```
ubuntu/v1/24/   # Configs specific to Ubuntu 24 systems only (eg. snap related configs)
init/v1/centos/ # Inherit and also it will add new configs such firewall
```

## Why I like this way?

* Keeps configs portable, consistent, and easy to roll back
* Makes automation scripts simpler by following predictable paths
* Supports multiple versions for safer upgrades or environment-specific tweaks


