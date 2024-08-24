# PLURA LOG COLLECTOR

## 1. dhcpd

### 1.1 Change log facility in dhcpd.conf
````
log-facility local6;
    
service dhcpd restart
````
### 1.2 Define facility local6 in rsyslog.conf
````
local6.*                                                -/var/log/dhcpd.log
    
service rsyslog restart
````
### 2. named

### 1.1 Run logstash for named
````
nohup /usr/share/logstash/bin/logstash -f /etc/logstash/conf.d/70-named-plura.conf > /var/log/plura/app-named-nohup.log 2>&1 &
````
