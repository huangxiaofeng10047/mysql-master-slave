# Master配置
[mysqld]
log-bin
bind-address=0.0.0.0
max_connections = 2000
skip-name-resolve
slave-skip-errors=all
wait_timeout = 1800
interactive_timeout = 1800
default-time-zone=+08:00
sort_buffer_size = 4M


# Slave配置
[mysqld]
super-read-only
bind-address=0.0.0.0
max_connections=1000
skip-name-resolve
slave-skip-errors=all
wait_timeout = 1800
interactive_timeout = 1800
default-time-zone=+08:00
sort_buffer_size = 4M