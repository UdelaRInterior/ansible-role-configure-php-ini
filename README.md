ansible-role-configure-php-ini
=========

Ansible role to configure php.ini file of our server in acordance to the listed on php_ini_parameters_and_values

Requirements
------------

Ansible >= 2.3

Role Variables
--------------

```yaml
# Full path to php.ini file
php_ini_path: /etc/php/7.0/cli/php.ini

# List of PHP parameter to configure
php_ini_parameters_and_values:
  - parameter: post_max_size
    value: 2G
  - parameter: upload_max_filesize
    value: 2G
```

Dependencies
------------

No dependences

Example Playbook
----------------

```yaml
- hosts: servers_lamp
  roles:
     - ansible-role-configure-php-ini
```

License
-------

(c) Universidad de la República (UdelaR), Red de Unidades Informáticas de la UdelaR en el Interior.
licenced under GPL-v3

Author Information
------------------

[santiagomr](https://github.com/santiagomr)
https://github.com/UdelaRInterior
https://proyectos.interior.edu.uy/
