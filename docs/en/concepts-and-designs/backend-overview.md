# Observability Analysis Platform
SkyWalking is an Observability Analysis Platform that provides full observability to services running in both brown and green zones, as well as services using a hybrid model.

## Capabilities
SkyWalking covers all 3 areas of observability, including, **Tracing**, **Metrics** and **Logging**.

- **Tracing**. SkyWalking native data formats, and Zipkin traces of v1 and v2 formats are supported.
- **Metrics**. SkyWalking supports mature metrics formats, including native meter format, OTEL metrics format, and Telegraf format.
SkyWalking integrates with Service Mesh platforms, typically Istio and Envoy, to build observability into the data plane 
or control plane. Also, SkyWalking native agents can run in the metrics mode, which greatly improves performances.
- **Logging**. Includes logs collected from disk or through network. Native agents could bind the tracing context with logs automatically,
or use SkyWalking to bind the trace and log through the text content.

There are 3 powerful and native language engines designed to analyze observability data from the above areas.
1. [Observability Analysis Language](oal.md) processes native traces and service mesh data.
1. [Meter Analysis Language](mal.md) is responsible for metrics calculation for native meter data, and adopts a stable and widely used metrics system, such as Prometheus and OpenTelemetry.
1. [Log Analysis Language](lal.md) focuses on log contents and collaborate with Meter Analysis Language.
