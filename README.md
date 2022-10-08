# Gitpod Launcher Example

This repository is a proof of concept launching a Gitpod workspace with a pre-determined config. 

## `.gitpod.yml` 

Reads a repo passed in via [URL environment variables](https://www.gitpod.io/docs/configure/projects/environment-variables#providing-one-time-environment-variables-via-url), clones it to the workspace, and replaces the launcher's contents and git context with the new repo

This should remain one single **command** where all instructions are performed sequentially. Any commands you want to run on first load should belong in this file

This file is single-use and deletes itself when it's done

## `.gitpod.template.yml`

Becomes the new `.gitpod.yml` for the repo

## Examples

### default (jacobparis/new, configured in yml)
[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/jacobparis/serverless-gitpod-launcher)

### jacobparis/react-boilerplate
[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#REPO=https%3A%2F%2Fgithub.com%2Fjacobparis%2Freact-boilerplate/https://github.com/jacobparis/serverless-gitpod-launcher)
