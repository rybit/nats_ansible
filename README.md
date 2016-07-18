This will configure a cluster of nats servers. It does by installing the versioned binary and then symlinking.

This also assumes that you'll be using TLS. And has paths appropriately for the clients.

The vars used:
  - tls_key_file
  - tls_cert_file
  - tls_ca_file
  - nats_install_dir
  - nats_port
  - nats_monitoring_port
  - nats_cluster_port
  - nats_version

It assumes that your nats servers will be in a block like this:
```
[nats]
nats1
nats2
```

