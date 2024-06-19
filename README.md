# Sofi Core GitOps

This repo contains the GitOps configuration for the Sofi Core application.

FluxCD is bootstrapped to track this repo for changes.

I've implemented the repository structure [recommended by FluxCD.](https://fluxcd.io/flux/guides/repository-structure/)

A base layer is set up which is adjusted by Kustomize for each environment.

When adding a new environment, make sure to add the configuration to the
GitHub actions workflow in the sofi_core repo. This needs to be done to enable
the image tages to be updated by the pipeline.
