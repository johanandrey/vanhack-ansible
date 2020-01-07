# vanhack-ansible

# @author: Johan Andrey Barón
# @email: johanandrey.baron@gmail.com
# @description: Ansible project for vanhack test


Play the whole project:
ansible-playbook site.yml --vault-password-file=.vault_pass.txt -v

Play Infra AWS + Deployment:
ansible-playbook site.yml --vault-password-file=.vault_pass.txt -t aws_setup -v 

Play only app changes:
ansible-playbook site.yml --vault-password-file=.vault_pass.txt -t aws_webapp -v

Play only database changes:
ansible-playbook site.yml --vault-password-file=.vault_pass.txt -t aws_db -v
