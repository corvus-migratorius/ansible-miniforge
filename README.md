Role Name
=========

A brief description of the role goes here.

Requirements
------------

None

Role Variables
--------------

`usernames`: a list of username strings 
`condarc.channels`: a list of Conda channel strings

Dependencies
------------

None

Example Playbook
----------------

```yaml
role:
  - role: miniforge
    usernames:
      - alice
      - bob
    condarc:
      channels: [ conda-forge ]
      dependencies: [ python=3.10, pip>=22.2, shellcheck==0.9.0, terraform==1.6.5 ]
```
----------------

```yaml
condarc_file: environment.yaml
```

As an alternative to the list of channels and dependencies, an environment file can be provided.

----------------

License
-------

BSD

Author Information
------------------

corvus-migratorius@proton.me
