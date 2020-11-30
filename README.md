Role Name
=========

A simple, opinionated ansible role to install unbound.

DNS-over-TLS is enforced, as well as DNSSEC. Some optional hardening
options are also enabled. Unbound is configured to listen locally only,
and `resolv.conf` is modified to send all local DNS requests to unbound.
Only port 853 over tcp needs to be allowed outbound for unbound to work
correctly.

Example Playbook
----------------

```yaml
- hosts: localhost
  roles:
      - capnspacehook.unbound
```

License
-------

MIT
