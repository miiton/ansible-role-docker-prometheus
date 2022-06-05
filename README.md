# docker-prometheus

## Role Variables

### prom_extra_hosts

```yml
prom_node_targets:
  - name: app01
    ipaddr: 192.168.0.1
    port: 9100
  - name: app02
    ipaddr: 192.168.0.2
    port: 9100
```

### prom_external_label

```yml
prom_external_label: mymon
```

### prom_httpcheck_targets

```yml
prom_httpcheck_targets:
  - https://app01.example.com/
  - https://app02.example.com/
```

### ec2 params

```yml
prom_ec2_monitoring_enable: true
prom_ec2_monitoring_access_key: AKIAIOSFODNN7EXAMPLE
prom_ec2_monitoring_secret_access_key: wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY
```
