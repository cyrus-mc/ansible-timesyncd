# Ansible Role : Container Linux systemd-timesyncd

An Ansible Role that configures/manages the systemd-timesyncd daemon on Container Linux.

## Role Variables:

Available variables are listed below, along with the default values (see `defaults/main.yml`):

    ntp_servers: [ 0.coreos.pool.ntp.org 1.coreos.pool.ntp.org 2.coreos.pool.ntp.org 3.coreos.pool.ntp.org ]

## Dependencies

None.

## Example Playbook

    - hosts: kubernetes-nodes
      var_files:
      - vars/main.yaml
      roles:
      - 'timesyncd'
