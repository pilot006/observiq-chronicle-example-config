# observiq-chronicle-example-config

Example 'config.yaml' configurations for bringing events in to Chronicle Security Operations leveraging BindPlane ObservIQ OpenTelemetry agents.

`config_windows.yaml` - Example configuration for Windows. Includes Windows Sysmon & Windows Event Logs

`config_nix.yaml` - Example configuration for *nix. Includes Linux Sysmon and auditd. **Note:** while not required, it is recommended to update the auditd.conf file to include the hostname in  the logs. Without this, the logs has no host correlation.

`auditd_extension.conf` - Chronicle parser extension to be used after [updating auditd configuration](https://man7.org/linux/man-pages/man5/auditd.conf.5.html) to include the hostname with the `name_format` configuration
