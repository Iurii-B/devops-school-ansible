In Hometask2 used two approaches:
- for Alice and Bob used a loop and inserted encrypted passwords directly into playbook; used the command "ansible all -i localhost, -m debug -a "msg={{ 'PASSWORD' | password_hash('sha512', 'mysecretsalt') }}""
- for Carol created a separate file vars/carols_password which contained just password string and encrypted it using Ansible Vault; used the command "
ansible-vault encrypt vars/carols_password --vault-password-file vault_pass"

The vault_pass file is excluded from GIT.
