
# Ansible role: `Secure Remote Docker daemon using SSL`

## Requirements

###Master
ansible V2.10.9

###Node
No requirements. The role will install Docker and all requirements before setting it up.

Requirements installation task is tested on centos v7 

## Role Variables

### Required parameters

* **passphrase:** unique passphrase for openssl private key

### Optional

* **docker_port[default=2376]:** Docker TCP port
* **certificates_dir[default=/etc/docker]:** Path to store certificates on the remote machine

## Example Playbook
```
- hosts: production

  vars:
    host_dns: "production"
    host_addr: "192.168.64.11"
    passphrase: "docker"
  roles:
    - role: docker-ssl
```
## License

MIT