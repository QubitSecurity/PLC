# PLURA LOG COLLECTOR

## 1. dhcpd

### 1.1 Change log facility in dhcpd.conf

    log-facility local6;
    
    service dhcpd restart

### 1.2 Define facility local6 in rsyslog.conf

    local6.*                                                -/var/log/dhcpd.log
    
    service rsyslog restart

### 2. named

### 1.1 Change logging in named.conf
