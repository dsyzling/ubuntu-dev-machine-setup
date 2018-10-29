# Ubuntu Developer Machine Setup With Ansible

Install some required setup tools.
  sudo apt install git ansible

git clone https://github.com/dsyzling/ubuntu-dev-machine-setup.git

cd ubuntu-dev-machine-setup
ansible-playbook site.yml -K


