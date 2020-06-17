**To execute on a server with sudo username and password**
ansible-playbook playbook.yml -i inventory.ini --user=username --extra-vars "ansible_ssh_user=userName ansible_ssh_port=1231 ansible_ssh_pass=sudopassword ansible_sudo_pass=sudopassword"
