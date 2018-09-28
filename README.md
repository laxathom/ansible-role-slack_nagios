Ansible Role for Nagios Slack notification
==========================================

Ansible role to install slack plugin for nagios and its associated crendentials

Requirements
------------
None.

Role Variables
--------------

Available variables are listed below, along with default values (see `defaults/main.yml`):

```yaml
slack_nagios_url: # Base url to download the pluging
slack_nagios_bindir: # Binary/dest dir where the plugin will be installed and run
slack_nagios_domain: # Your slack workspace url
slack_nagios_token: # Your slack integration token.
```

Dependencies
------------

None.

Example Playbook
----------------

```yaml
    - hosts: nagios-servers
      roles:
         - { role: laxathom.slack_nagios }
```

License
-------

MIT
