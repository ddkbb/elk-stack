# Auditbeat
for linux

# filebeat

### creating a keystore
`filebeat keystore create`<br>
`filebeat keystore add ES_PWD`<br>
`filebeat keystore list`

In the configuration file, use password: "`${ES_PWD}`"

To test the configuration file
`cd /usr/share/filebeat/bin`
`filebeat test config -e`

### setup
must configure auditbeat.yml to forward files to elasticsearch
/etc/filebeat/filebeat.yml



### References
- https://www.elastic.co/guide/en/beats/filebeat/8.11/filebeat-installation-configuration.html

default paths

- https://www.elastic.co/guide/en/beats/auditbeat/current/directory-layout.html

keystore creation
 - https://www.elastic.co/guide/en/beats/auditbeat/8.11/keystore.html

# metricbeat
for docker logging

# winlogbeat
for windows
