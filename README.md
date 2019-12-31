# vanhack-ansible

# @author: Johan Andrey Barón
# @email: johanandrey.baron@gmail.co
# @description: Ansible project for vanhack test



ami -> vpc -> cloudformation -> elb

Play:
ansible-playbook site.yml --vault-password-file=.vault_pass.txt