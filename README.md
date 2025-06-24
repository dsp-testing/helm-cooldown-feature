# Helm Dependencies That Need Updates

## complex/chart.yml

Dependencies that need updates:
- redis (version 17.11.3)
- rabbitmq (version 11.16.2)
- postgresql (version 12.5.7)
- mongodb (version 13.9.1)
- kafka (version 23.0.7)
- elasticsearch (version 19.5.10)
- kibana (version 10.4.2)
- prometheus (version 19.6.1)
- grafana (version 6.59.0)
- jaeger (version 0.71.3)
- cert-manager (version 1.12.3)

## nested/values.yaml

While values.yaml doesn't directly specify the dependency versions (those are in Chart.yaml), the following configurations are present and may need corresponding updates when dependencies are updated:

- redis configuration
- rabbitmq configuration
- postgresql configuration
- mongodb configuration
- kafka configuration
- elasticsearch configuration in the elastic-stack section
- kibana configuration in the elastic-stack section
- prometheus configuration in the monitoring section
- grafana configuration in the monitoring section
- jaeger configuration in the tracing section

The image referenced in the values.yaml also needs an update:
- example/microservice-app:1.4.2

## v2/requirements.yml

Dependencies that need updates (Helm v2 style):
- nginx-ingress (version 4.7.1)
- cert-manager (version 1.12.3)
- prometheus (version 19.6.1)
- grafana (version 6.59.0)
- elasticsearch (version 7.17.3)
- fluentd (version 2.6.2)
- kibana (version 7.17.3)

## v3/Chart.yaml

Dependencies that need updates (Helm v3 style):
- redis (version 17.11.3)
- postgresql (version 12.5.7)
- mongodb (version 13.9.1)

The appVersion field may also need an update:
- appVersion: "1.16.0"
