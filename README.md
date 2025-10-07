## Install any software

    ansible-playbook -i hosts.yml playbooks/install_software.yml -e "packages=['nginx','git']"

## Install pyenv and any python version

Depends on `agoloncser.pyenv` role

    ansible-playbook -i hosts.yml playbooks/pyenv.yml