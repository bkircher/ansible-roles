# volatile-journal

Set journald `Storage=` configuration explicitly to "volatile".

Also mask rsyslog.service. We do not need persistent logs since we only care for the current boot or have something like fluent-bit.service write logs away on the network.

## References
- `journald.conf(5)`
- `journald.conf.d(5)`
- https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/8/html/configuring_basic_system_settings/optimizing-systemd-to-shorten-the-boot-time_configuring-basic-system-settings
- https://wiki.archlinux.org/title/Systemd/Journal
