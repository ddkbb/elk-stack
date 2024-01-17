# Elastic Search

### allowing SHA1 signed packages
change to allow sha1
  update-crypto-policies --set DEFAULT:SHA1
change back after reboot  
  update-crypto-policies --set DEFAULT
download key
  rpm --import https://artifacts.elastic.co/GPG-KEY-elasticsearch
https://www.elastic.co/guide/en/elasticsearch/reference/current/rpm.html
https://www.redhat.com/en/blog/rhel-security-sha-1-package-signatures-distrusted-rhel-9

### Resetting password
/usr/share/elasticsearch/bin/elasticsearch-reset-password -u <user> -i --url https://localhost:<port>

### turning off logging to set environment variables
To turn off
` set +o history `
Set environment variable here
To turn on
` set -o history `

### References
- https://www.elastic.co/guide/en/elasticsearch/reference/current/rpm.html
- https://discuss.elastic.co/t/bin-elasticsearch-setup-passwords-no-such-file-or-directory/247725
- https://stackoverflow.com/questions/72235201/elasticsearch-password-reset-failing-with-https
