ansible-role-linkding
=========

A very simple role to run linkding in a docker container

Requirements
------------

Docker and all dependencies to manage docker containers need to be installed on the target machine for this role to be working.

Role Variables
--------------

| Variable                  | Description                                   | Default               |
|---------------------------|-----------------------------------------------|-----------------------|
| linkding_filesystem_root  | The filesystem root for linkding data         | /srv/volumes/linkding |
| linkding_container_name   | The container name for the linkding container | linkding              |
| linkding_image_name       | The imag used for the linkding container      | sissbruecker/linkding |
| linkding_image_tag        | The tag used for the linkding container       | latest                |
| linkding_config_http_port | The host port for the web UI                  | 3000                  |

Example Playbook
----------------

```yaml
- hosts: servers
  roles:
     - linkding
```

License
-------

MIT

