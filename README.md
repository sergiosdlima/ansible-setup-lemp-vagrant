# Ansible LEMP setup with Vagrant

O Vagrant irá criar um ambiente Ubuntu 20.04 para provisionamento com Ansible de um ambiente Linux com Nginx, Mysql e PHP.

## Como executar

1. Crie o ambienete ubuntu com o comando `vagrant up`.
2. Execute a receita setup.yml com o ansible com o comando `ansible-playbook -i hosts setup.yml`.

Obs: Se der problema man in the middle por conta da chave ssh, execute o comando `ssh-keygen -f "/home/sergio/.ssh/known_hosts" -R "10.10.10.30"`.

## Como remover

Execute o comando `vagrant destroy -f` para remover o servidor.