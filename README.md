# Containerized Application Collaboration Examples for WebMethods

## Overview

This repository is a collection of examples showing use cases where webMethods products work together between themselves or with other products for typical purposes such as metrics gathering, service audit and so on.

The examples are built to be run quickly, with a general approach like

- clone repo
- go to your example of choice
- copy `EXAMPLE.env` into `.env`
- set the necessary parameters in the `.env` file 
  - e.g. set the product license
- run the example
  - e.g. `docker compose up`
- inspect the result and the way it is achieved by reading the provided documentation and code examples

The benefits of having these examples are:

1. Exploit containers and IaC to quickly start a playground for a specific use case
2. Explore the product's characteristics and behavior for the given use case
3. Have a starting point for your code: just copy and evolve, respecting the original license
4. Build quick and easily repeatable repro cases in case of issues
5. Build quickly Spikes and POVs
6. Keep your machine clean, and eventually explore ephemeral environments, as the examples are containerized and the instances can be pruned in a blink of an eye
7. Borrow the patterns for non containerized deployments too. Although the examples are containerized, for productivity reasons, many of the examples can be used on traditional fixed landscapes deployments too

------------------------------

These tools are provided as-is and without warranty or support. They do not constitute part of the Software AG product suite. Users are free to use, fork and modify them, subject to the license agreement. While Software AG welcomes contributions, we cannot guarantee to include every contribution in the master project.
