# Kibana

### Configurations
using ssl, change
https://www.elastic.co/guide/en/kibana/8.11/production.html#openssl-legacy-provider

### Token generation
```
/usr/share/elasticsearch/bin/elasticsearch-create-enrollment-token -s kibana
```
```
/usr/share/kibana/bin/kibana-setup --enrollment-token
```
https://www.elastic.co/guide/en/elasticsearch/reference/current/configuring-stack-security.html

### Accessing Kibana
` http://localhost<port> `
https://www.elastic.co/guide/en/kibana/current/access.html

### References
- https://www.elastic.co/guide/en/kibana/current/rpm.html
