nagios-plugins
=========

Ansible role to copy custom Nagios compatible plugins to remote

Role Variables
--------------

The following variables must be declaterd on hostvars or group_vars in order for the role to work.

```
nagios_plugins_custom_dir_src: group_files/Ubuntu-16/nagios-plugins/custom
nagios_plugins_custom_dir_dest: /usr/lib/nagios/plugins
```

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```
Example:
group_vars/Ubuntu-16/vars.yml
nagios_plugins_custom_dir_src: group_files/Ubuntu-16/nagios-plugins/custom
nagios_plugins_custom_dir_dest: /usr/lib/nagios/plugins


some_playbook.yml
- hosts: my-app-nodes
  become: yes
  roles:
    - nagios-plugins
```

License
-------

MIT

Author Information
------------------

Tal Lannder TLannder@globeandmail.com
