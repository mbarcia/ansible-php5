Webhop - PHP5 Ansible Role
==========================

Installs the latest PHP5 and associated packages on an ubuntu host.
Automatically dimension max_children limit on startup time.

## Role Variables

##### Defaults

- `php_version` - The version of PHP to install. (**5.6**)
- `php_post_max_size` - Max size (in Mb) for POST requests. (**30**)
- `php_upload_max_filesize` - Max size (in Mb) for uploads. (**30**)
- `php_pm_max_children` - FPM max children. (**10**)
- `create_virtualenv` - Create a virtualenv (**true**)
- `scripts_dir` - Path to install scripts into (**/opt/beamly/scripts**)
- `virtualenv_dir` - Path to create virtualenv in (**/opt/beamly/virtualenvs**)
- `scripts_owner` - User to chown the scripts (**ubuntu**)
- `scripts_group` - Group to chown the scripts (**ubuntu**)
- `fpm_total_ram_slice` - Ratio/slice of memory allocated to PHP-FPM (**0.4**)
- `fpm_confpath` - PHP-FPM configuration file path (**/etc/php5/fpm/pool.d/www.conf**)
- `fpm_avgmem` - Average memory footprint of a PHP-FPM child thread (**128**)

Usage
-----

```yaml
roles:
    - { role: webhop.php5, fpm_avgmem: 90 }
```

Author Information
-------------------

* Chris Warren - chris@beamly.com
* Neil Saunders - neil@beamly.com
* Mariano Barcia - mariano.barcia@beamly.com
* Vik Bhatti - vik@beamly.com
