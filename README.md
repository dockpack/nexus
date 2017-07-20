Nexus
=========

Sonatype Nexus Repository Manager 3

Requirements
------------

n/a

Role Variables
--------------

```
# from defaults/main.yml
nexus_version:
nexus_workdir: /opt/nexus/sonatype-work/nexus3
nexus_piddir: /var/run/nexus
nexus_user: nexus
nexus_group: nexus

# from vars/main.yml
nexus_name: "nexus-{{ nexus_version }}"
nexus_tarfile: "{{ nexus_name }}-unix.tar.gz"
nexus_base_url: https://download.sonatype.com/nexus/3
nexus_url: "{{ nexus_base_url }}/{{ nexus_tarfile }}"

nexus_location: /opt/nexus
nexus_home: "{{ nexus_location }}/{{ nexus_name }}"

nexus_context_path: /
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
