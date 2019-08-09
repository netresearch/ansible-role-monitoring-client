# ansible-role-monitoring-client

Sets up [NodeExporter](https://github.com/prometheus/node_exporter) + [cAdvisor](https://github.com/google/cadvisor) docker containers using the configuration of [stefanprodan's dockprom](https://github.com/stefanprodan/dockprom).

## Exaple playbook

```yaml
---

- name: Monitoring Clients
  hosts: database, webserver
  roles:
    - roles/external/ansible-role-monitoring-client
```
