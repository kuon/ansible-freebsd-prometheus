
# THIS REPOSITORY HAS MOVED

New URL: https://git.goyman.com/kuon/ansible-freebsd-prometheus

Why I moved everything out of GitHub:

https://github.com/kuon/WhyILeftGithub/blob/main/README.md

----

FreeBSD-prometheus
==================

Install prometheus and collectd exporter.


This role contains a minimal default prometheus config, you will want to override it.


**DISCLAIMER**: This role has been created for my personal use and come with
no warranty. This role is very opiniated and may cause trouble with your install.

**NOTE**: This roles distributes a binary of collectd_exporter. Compiled from https://github.com/prometheus/collectd_exporter/tree/5974601cc73156a168e1e2b2657131bd5259c08e


Requirements
------------

FreeBSD, runit

Role Variables
--------------


- `prometheus_directory`, install directory of prometheus, default to `/srv/prometheus`.
- `prometheus_version`, version of prometheus to install, default to `0.17.0`.
- `prometheus_collectd_port`, port of the collectd network listener, default to `25826`.
- `prometheus_custom_config`, custom config file path to be used instead of the default one.


License
-------

MIT

Author Information
------------------

Ansible role by Nicolas Goy @kuon.

