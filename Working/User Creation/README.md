# Ansible - Playbook

### Playbook to create a user to be useful for automating further tasks
<br>

To run the playbook
```bash
ansible-navigator run -m stdout creating_ansible_user.yml --ask-become-password
```
```bash
ansible-playbook creating_ansible_user.yml --ask-become-password
```
<br>

Important things to change in the files

1. username in ansible.cfg
2. user_password in creating_ansible_user.yml file
3. pub_url in creating_ansible_user.yml file
4. Enter the ip set or single ip in inventory file
<br>

Methods to pass the sudo passwords

1. By using `--ask-become-password`
2. - store the password in a file 
   - pass the file by `--become-password-file=<file>`