Ansible Examples
================

Install ansible with ``pip``::

  python -m pip install ansible


List modules::

  ansible-doc -l

Pull up documentation & examples on a module::

  ansible-doc command

Example of pinging all hosts in inventory (ssh connect)::

  ansible -i inventory_example.ini all -m ping

Run command via SSH::

    ansible -i inventory_example.ini all -a "free -h"
    ansible -i inventory_example.ini all -m command -a "free -h"

Run playbook::

  ansible-playbook example_playbook.yml -f 10 -i inventory.ini


References
----------

- https://docs.ansible.com/