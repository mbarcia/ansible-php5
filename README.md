Webhop - PHP5 Ansible Role
==========================

Installs the latest PHP5 and associated packages on an ubuntu host

## Role Variables

##### Defaults

- `php_version` - The version of PHP to install. (**5.6**)
- `php_post_max_size` - Max size (in Mb) for POST requests. (**30**)
- `php_upload_max_filesize` - Max size (in Mb) for uploads. (**30**)

Usage
-----

```yaml
roles:
    - { role: webhop.php5 }
```

Author Information
-------------------

* Chris Warren - chris@beamly.com
* Neil Saunders - neil@beamly.com
