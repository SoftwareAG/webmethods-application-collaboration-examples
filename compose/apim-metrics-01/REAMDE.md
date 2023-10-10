# Example 01 for Metrics Centralization for Software AG API Management

This example is provided for two main reasons:

1. to show the consultant and eventually the customer how the metrics are gathered using Prometheus and shown using Grafana.
2. to provide a starting point for the development of real-world solutions.

## Quick Start

This example is a docker compose project, therefore the user must have a machine where they can run docker compose and browser instances to play around with the dashboards and administration interfaces.

Follow the general steps below

- Procure valid licenses for the involved products: 
  - API Gateway, Developer Portal
- Ensure you have access to container images for the involved products: 
  - API Gateway, Developer Portal, Elasticsearch, Kibana, Prometheus, Grafana
- Clone this repository
- Copy `EXAMPLE.env` into `.env`
- Ensure the resources prerequisites are satisfied, for example ensure Elasticsearch need to have the kernel parameter `vm.max_map_count` set to at least a value of `262144`
  - An example on how to do this is [here](https://github.com/SoftwareAG/sag-unattended-installations/tree/main/04.support/alpine-set-elk-prerequisites)