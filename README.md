# docker-prometheus

## Role Variables

```yml
prom_scrape_interval: 60s
prom_retention_time: 15d
prom_samehost: true
prom_network_subnet: 192.168.100.0/24
prom_node_targets:
  - name: app01
    ipaddr: 192.168.0.1
    port: 9100
  - name: app02
    ipaddr: 192.168.0.2
    port: 9100
prom_external_label: mymon
prom_cadvisor_targets:
  - cadvisor.example.com:8080
prom_httpcheck_targets:
  - https://app01.example.com/
  - https://app02.example.com/
prom_ec2_monitoring_enable: true
prom_ec2_monitoring_region: ap-northeast-1
vault_host: vault.example.com # if need
blackbox_exporter_host: blackbox_exporter:9115
```

### Environment

```
AWS_ACCESS_KEY: AKIAIOSFODNN7EXAMPLE
AWS_SECRET_ACCESS_KEY: wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY
```
