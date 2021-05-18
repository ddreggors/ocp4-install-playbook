# The install playbook

This playbook aims to be a complete installer that uses hashicorp vault to store secrets like the ssh key, certificates, and passwords for VCSA


## The variables you can override



| Variable          | Default Value |
| :---              | :---:         |
| clean_install_dir | true          |
| mirror_repo       | false         |
| download          | true          |
| install           | false         |
| vtoken            |               |


## Running the playbook


To just create the install config and not run the install:

`ansible-playbook ./main.yaml -e vtoken=<your vault token>`

or to create the install config, do not attempt to check or download the installer (already downloaded) and proceed with install:

`ansible-playbook ./main.yaml -e vtoken=<your vault token> -e download=false -e download=false`
