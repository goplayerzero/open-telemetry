# OpenTelemetry ➜ PlayerZero
Export OpenTelemetry Logs into [PlayerZero](https://go.playerzero.app/)


### Overview
The PlayerZero exporter is an otlphttp exporter for logs with a fatal or error status. You can configure it through environment/system variables, a config file, or however else you have setup your OpenTelemetry agent. If you have not yet set up OpenTelemetry [check out the docs](https://opentelemetry.io/docs/getting-started/dev/) or see if one of [our other connectors](https://go.playerzero.app/connectors) makes more sense.


### Configuration
`Endpoint` = "https://sdk.playerzero.app/otlp"

`Headers` =  {"Authorization": "Bearer \<your-playerzero-api-token>"}


### Config File Example
Copy the following into your OpenTelemetry config.yml file
```
exporters:
  otlphttp/playerzero:
    endpoint: "https://sdk.playerzero.app/otlp"
    headers:
      Authorization: "Bearer <your-playerzero-api-token>"
```
