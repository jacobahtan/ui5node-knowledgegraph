# Smart Advisory Companion: A Node.js Microservice on Cloud Foundry

...

> [!IMPORTANT]
Work in Progress

## Business Scenario
wip

## Persona
wip

## Solution Architecture
wip
<!-- [<img src="https://github.com/SAP-samples/btp-generative-ai-hub-use-cases/assets/8436161/a826c07b-304e-4849-9ac0-493a739536d6"/>](https://github.com/SAP-samples/btp-generative-ai-hub-use-cases/assets/8436161/a826c07b-304e-4849-9ac0-493a739536d6) -->

## Pre-requisites
Below are some setup steps that are required to ensure a success deployment of the application.
- make sure the python endpoint is up and running.

## Steps to Run Locally (for development)
- create an .env file in root level
- in the .env file, have the following values PY_ENDPOINT="https://indb-embedding.cfapps.eu12.hana.ondemand.com"
- you may refer to .env_sample.
- npm install
- to run locally: node app.js

## Steps to Deploy
- cf login
- cf push ui5node-poc-knowledgegraph -k 256MB -m 256MB
- cf set-env ui5node-poc-knowledgegraph PY_ENDPOINT https://indb-embedding.cfapps.eu12.hana.ondemand.com
- cf restart ui5node-poc-knowledgegraph

### todo
- [done] decouple env variables