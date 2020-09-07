# NATS Exporter Ansible Role

NATS.io is a simple, secure and high performance open source messaging system for cloud native applications, IoT messaging, and microservices architectures.

## Installation

``` yaml
# requirments.yaml
- src: git@github.com:4lie/ansible-role-prometheus-nats-exporter.git
  scm: git
  version: master
  name: prometheus-nats-exporter
```

## Role Variables

``` yaml
prometheus_nats_exporter_version: "0.6.2"
prometheus_nats_exporter_exec_parameters: "-channelz -connz -routez -serverz -subz -varz"
prometheus_nats_exporter_nats_server_address: "http://127.0.0.1:8222"
```

## Example Playbook

``` yaml
- hosts: servers
  roles:
    - prometheus-nats-exporter
```
