# Example 02 for Metrics Centralization for Software AG UniversalMessaging

## Purpose
1. Start UniversalMessaging (single server) in a container
2. Collect metrics from UniversalMessaging server using JMX Exporter that can be used to gather data from MBeans of a JMX target. The JMX Exporter is included in the Universal Messaging product delivery as the jar file jmx_prometheus_javaagent.jar. You can run the JMX Exporter as a Java аgent to export a set of Universal Messaging time series data that can be analyzed by Prometheus.
   - [JMX_Exporter_Metrics](https://documentation.softwareag.com/universal_messaging/num10-15/webhelp/num-webhelp/#page/num-webhelp%2Fre-jmx_exporter_metrics.html%23)
## Quick Start/ How to
This example is a docker compose project, therefore the user must have a machine where they can run docker compose and browser instances to play around with the dashboards and administration interfaces. As soon as the example is using DockerImages from the Software AG Container Registry , the user needs an initialized access to the SAG Container Registry.

Follow the general steps below:
1. Provide a valid license file for Software AG UniversalMessaging under compose/um-metrics-02/um.
2. Ensure you have access to container images for the involved products: 
    - Software AG UniversalMessaging, Prometheus, Grafana, Google cAdvisor.
3. Clone this repository.
4. Optional: Copy `EXAMPLE.env` into `.env`.
5. Navigate to `compose/um-metrics-02`.
6. Execute `docker-compose up` or `docker-compose --env-file EXAMPLE.env up` if Step 4 skipped.