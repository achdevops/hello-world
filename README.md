# Neuvector Scan - Github Actions

## Pre-requisites
- Create a environment secret with github token
- adjust the image name and tag as input parameters to the scan stage
- adjust the registry credentials (ghcr, dockerhub ...)
- set the criteria on the env vars section

## Stages
- Build a simple python hello-world app (flask)
- Run a temporal standalone NV Scanner
- Scan the local image and generate the json vulnerabilities report
- Create a CSV Report Artifact
- Check the criteria for By Name, HIGH or MED Vulnerabilities from the report
- if criteria pass, push the image to the registry.