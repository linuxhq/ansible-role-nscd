# ansible-role-nscd

[![Build Status](https://travis-ci.org/linuxhq/ansible-role-nscd.svg?branch=master)](https://travis-ci.org/linuxhq/ansible-role-nscd)

RHEL/CentOS - Name service cache daemon

## Requirements

None

## Role Variables

Available variables are listed below, along with default values:

    nscd_debug_level: 0
    nscd_logfile: /var/log/nscd.log
    nscd_max_threads: 32
    nscd_paranoia: False
    nscd_reload_count: 5
    nscd_restart_interval: 3600
    nscd_server_user: nscd
    nscd_threads: 4
    nscd_group_auto_propagate: True
    nscd_group_check_files: True
    nscd_group_enable_cache: True
    nscd_group_max_db_size: 33554432
    nscd_group_negative_time_to_live: 60
    nscd_group_persistent: True
    nscd_group_positive_time_to_live: 3600
    nscd_group_shared: True
    nscd_group_suggested_size: 211
    nscd_hosts_check_files: True
    nscd_hosts_enable_cache: True
    nscd_hosts_max_db_size: 33554432
    nscd_hosts_negative_time_to_live: 20
    nscd_hosts_persistent: True
    nscd_hosts_positive_time_to_live: 3600
    nscd_hosts_shared: True
    nscd_hosts_suggested_size: 211
    nscd_netgroup_check_files: True
    nscd_netgroup_enable_cache: True
    nscd_netgroup_max_db_size: 33554432
    nscd_netgroup_negative_time_to_live: 20
    nscd_netgroup_persistent: True
    nscd_netgroup_positive_time_to_live: 28800
    nscd_netgroup_shared: True
    nscd_netgroup_suggested_size: 211
    nscd_passwd_auto_propagate: True
    nscd_passwd_check_files: True
    nscd_passwd_enable_cache: True
    nscd_passwd_max_db_size: 33554432
    nscd_passwd_negative_time_to_live: 20
    nscd_passwd_persistent: True
    nscd_passwd_positive_time_to_live: 600
    nscd_passwd_shared: True
    nscd_passwd_suggested_size: 211
    nscd_services_check_files: True
    nscd_services_enable_cache: True
    nscd_services_max_db_size: 33554432
    nscd_services_negative_time_to_live: 20
    nscd_services_persistent: True
    nscd_services_positive_time_to_live: 28800
    nscd_services_shared: True
    nscd_services_suggested_size: 211

## Dependencies

None

## Example Playbook

    - hosts: servers
      roles:
        - role: linuxhq.nscd
          nscd_debug_level: 1
          nscd_logfile: /tmp/nscd.log

## License

BSD

## Author Information

This role was created by [Taylor Kimball](http://www.linuxhq.org).
