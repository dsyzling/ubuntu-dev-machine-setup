# Ubuntu cloudinit 

Create a cloudinit setup file and store under your user profile within Windows, e.g. Ubuntu-24.04.user-data.

Then from powershell run:
Ubuntu-24.04 

See:
https://documentation.ubuntu.com/wsl/en/latest/tutorials/cloud-init/
https://cloudinit.readthedocs.io/en/latest/reference/examples.html


# Ubuntu Developer Machine Setup With Ansible

Install some required setup tools.
  sudo apt install git ansible

git clone https://github.com/dsyzling/ubuntu-dev-machine-setup.git

cd ubuntu-dev-machine-setup
ansible-playbook wsl.yml -K --extra-vars "dssecretspass='password here'"
Run shell:
zsh 

# Post Installation Emacs initialisation 

Running Emacs for the first time will install all our required packages. Fonts need to be installed for icons used with lsp-mode, vertico, treemacs.

Run: M-x all-the-icons-install-fonts

Install pyright LSP server for python 
M-x lsp-install-server 
select pyright 
