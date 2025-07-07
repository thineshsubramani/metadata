# Metadata

This repo holds all the metadata for my system sync engine.
It helps me centrally manage configurations for all my systems, complete with versioning in sub-directories similar to how APIs are structured.
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

## Why this approach?

* Keeps configs portable, consistent, and easy to roll back
* Makes automation scripts simpler by following predictable paths
* Supports multiple versions for safer upgrades or environment-specific tweaks


