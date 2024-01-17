# Logstash

### checking if it works
```
/usr/share/logstash/bin/logstash -e 'input { stdin { } } output { stdout {} }'
```
- https://www.elastic.co/guide/en/logstash/8.11/first-event.html

### setting up logstash keystore
```
set +o history
export LOGSTASH_KEYSTORE_PASS=mypassword
set -o history
sudo -E /usr/share/logstash/bin/logstash-keystore --path.settings /etc/logstash create
```

### References
- https://www.elastic.co/guide/en/logstash/current/installing-logstash.html
- https://www.elastic.co/guide/en/logstash/current/keystore.html#keystore-password
- https://discuss.elastic.co/t/not-a-valid-logstash-keystore-error/159945
