# Ansible playbook which deploy nginx docker image

---

1. You need to setup hosts file production - replace PROD_HOST with your server ip or domain name.
2. You need to setup ssh key group_vars\webservers\vars.yml\ansible_ssh_private_key

Run command

`ansible-playbook -i production site.yml --limit webservers --ask-vault-password`

---

vault password: passw0rd

http access credentials: admin:passw0rd

repository with dockerfile - https://github.com/yorni/nginxImage
