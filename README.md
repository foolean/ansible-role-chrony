# ansible-role-chrony

    Ansible role to manage chrony

    Note: This role will mask systemd-timesyncd and remove ntp

## Requirements

    None


## Dependencies

    None


## Role Variables


**chrony_allow**

    List of clients permitted to query this server
    (default: null)

**chrony_driftfile**

    The name and path of the frequency file.
    (default: /var/lib/chrony/drift)

**chrony_keys**

    List of lines to be added to the keys file
    (default: null)

**chrony_listen**

    Interface chrony will listen on only accept requests on this interface.
    (default: null)

**chrony_logconfig**

    Specify which events chronyd will log
    (default: measurements statistics tracking)

**chrony_peers**

    List of NTP peers to query
    (default: null)

**chrony_servers**

    List of NTP servers to query
    (default: [0-3].pool.ntp.org)


## Example playbook

    ```yaml
    ---
    - hosts: all

      roles:
          - foolean/chrony
    ```


## Supported operating systems

    * Debian (11)
    * RedHat (8)
    * Rocky (8)
    * Raspbian (11)


## Compliance

    * CIS Debian Linux 11 Benchmark v1.0.0
    * CIS RedHat Enterprise Linux 8 Benchmark v2.0.0
    * CIS Rocky Linux 8 Benchmark v1.0.0


## License

    BSD-3-Clause
