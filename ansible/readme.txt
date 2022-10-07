ansible-playbook name.yml --extra-var "MYHOSTS=linux_servers"


Create an encrypted file
# ansible-vault create vault.yml
# ansible-vault create --vault-id password@prompt vault.yml 
Editing the encrypted file
# ansible-vault edit secure.yml
Decrypting a file
# ansible-vault decrypt secure.yml
Decrypt a running playbook
# ansible-playbook --ask-vault-pass email.yml
Create an encrypted string
# ansible-vault encrypt_string
# echo -n "secretword" | ansible-vault encrypt_string
