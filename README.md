
# Ansible role: `Secure Remote Docker daemon using SSL`

## Requirements
#Master
ansible V2.10.9

#Node
No requirements. The role will install Docker before setting it up.

## Role Variables

### Required parameters

* **passphrase:** passphrase for openssl private key

### Optional

* **docker_port:** 2376
* **certificates_dir[default=/docker-ssl]:** Path to store certificates on the remote machine

## Example Playbook

## License

MIT