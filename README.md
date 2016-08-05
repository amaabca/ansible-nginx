Ansible-Nginx
=============

This role sets up an nginx web server on ubuntu 16.04 with SSL.

Role Variables
--------------
Store the following in [a vault file](http://docs.ansible.com/ansible/playbooks_vault.html):

```yaml
ssl_private_key: |
-----BEGIN RSA PRIVATE KEY----
...
-----END RSA PRIVATE KEY----
app_name: my_app
nginx_template_path: /path/to/my/template
```

Example Playbook
----------------

```bash
ansible-playbook tests/test.yml -i your_inventory_file
```

How to include this role:

```yaml
- hosts: servers
  roles:
    - ansible-nginx
```

License
-------

MIT

Author Information
------------------

www.ama.ab.ca, webmaster@ama.ab.ca
