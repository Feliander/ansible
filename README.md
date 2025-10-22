## Ping

    ansible all -m ping

## Install any software

    ansible-playbook -i hosts.yml playbooks/install_software.yml -e "packages=['nginx','git']"

## Install pyenv and any python version

Depends on `agoloncser.pyenv` role

    ansible-playbook -i hosts.yml playbooks/pyenv.yml -e "version=3.12 global=true"

## Configure nginx server

    ansible-playbook -i hosts.yml playbooks/nginx.yml
