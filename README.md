# ansible-kibana

An Ansible role for installing [Kibana](http://www.elasticsearch.org/overview/kibana/).

## Role Variables

- `kibana_version` - Kibana version to install (default: `4.0.1`)
- `kibana_os` - Kibana operating system build (default: `linux`)
- `kibana_arch` - Kibana architecture build (default: `x64`)
- `kibana_dir` - Directory to extract the Kibana archive (default: `/opt`)
- `kibana_host` - Kibana address to bind to (default: `0.0.0.0`)
- `kibana_port` - Kibana port (default: `5601`)
- `kibana_elasticsearch` - ElasticSearch endpoint (default: `http://localhost:9200`)
- `kibana_index` - Name of Kibana index in ElasticSearch (default: `.kibana`)
- `kibana_log` - Kibana log path (default: `/var/log/kibana.log`)
- `kibana_log_rotate_count` - Kibana log rotation count (default: `5`)
- `kibana_log_rotate_interval` - Kibana log rotation interval (default: `daily`)
- `kibana_ca` - Certificate
- `kibana_ssl_key_file` - Key file
- `kibana_ssl_cert_file` - Cert file
- `kibana_verify_ssl` -  set to false to have a complete disregard for the validity of the SSL cert.
- `kibana_elasticsearch_username` - basic auth for maintaining the ```kibana_index```
- `kibana_elasticsearch_password` - basic auth for maintaining the ```kibana_index```


See the [examples](./examples/) directory.
