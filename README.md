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

`ansible-playbook ./main.yaml -e vtoken=<your vault token>`
