# PLURA LOG COLLECTOR

## 1. dhcpd

### 1.1 Change log facility in dhcpd.conf

    log-facility local6;

### 1.2 Define facility local6 in rsyslog.conf

    local6.*                                                -/var/log/dhcpd.log

### 2. named

### 1.1 Change logging in named.conf
