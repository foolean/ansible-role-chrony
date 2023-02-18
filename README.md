# ansible-role-chrony

Ansible role to manage chrony


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
    (default: [0-3].rhel.pool.ntp.org)


## Example playbook

    ```yaml
    ---
    - hosts: all

      roles:
          - foolean/chrony
    ```


## Compliance

    * CIS RedHat Enterprise Linux 8 Benchmark v2.0.0


## License

    BSD-3-Clause
