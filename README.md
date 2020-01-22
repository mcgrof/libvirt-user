libvirt-user
============

The ansible libvirt-user role lets you get install libvirt, and then configures
the system to allow the current user to set up guests.

Most ansible roles available for libvirt either install libvirt or configures
libvirt with many options and bells and whistles. All you really need for a
simple set up however, is to install libvirt and enable a regular user to use
libvirt.

This role installs libvirt and configures the current running user to be able
to use KVM via libvirt with the typical distro defaults.

Requirements
------------

Run a supported OS/distribution:

  * SUSE SLE / OpenSUSE
  * Red Hat / Fedora
  * Debian / Ubuntu

Role Variables
--------------

None.

Dependencies
------------

None.

Example Playbook
----------------

Below is an example playbook, say a bootlinux.yml file:

```
---
- hosts: localhost
  roles:
    - role: mcgrof.libvirt-user
```

License
-------

GPLv2
