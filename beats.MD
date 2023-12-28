# Auditbeat
for linux

# filebeat

### creating a keystore
`filebeat keystore create`<br>
`filebeat keystore add ES_PWD`<br>
`filebeat keystore list`

In the configuration file, use password: "`${ES_PWD}`"

To test the configuration file<br>
`cd /usr/share/filebeat/bin`<br>
`filebeat test config -e`

### setup
must configure filebeat.yml to forward files to elasticsearch
/etc/filebeat/filebeat.yml

change directory to the filebeat bin installation
`cd /usr/share/filebeat/bin` <br>
list modules <br>
`filebeat modules list` <br>
enable modules <br>
`filebeat modules enable <module>` <br>
- https://www.elastic.co/guide/en/beats/filebeat/current/filebeat-installation-configuration.html



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
