nexus
=========

Sonatype Nexus Repository Manager 3

Requirements
------------

n/a

Role Variables
--------------

```
nexus_version: 3.4.0-02
nexus_work: /opt/nexus/sonatype-work/nexus3
nexus_user: nexus
nexus_group: nexus
```

Dependencies
------------

[bbaassssiiee/base_java8](https://github.com/bbaassssiiee/base_java8/releases)

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
        - role: bbaassssiiee.nexus

License
-------

BSD

Author Information
------------------

Bas Meijer: [bbaassssiiee](https://github.com/bbaassssiiee)
