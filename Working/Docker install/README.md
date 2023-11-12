# Ansible - Playbook

### Playbook to install docker in any OS
<br>

To run the playbook
```bash
ansible-navigator run -m stdout docker_install.yml --ask-become-password
```
```bash
ansible-playbook docker_install.yml --ask-become-password
```
<br>

**Important things to note !!**

1. username = ansible (change if you insist)
2. Change the username in playbook to add in secondary group 


<br>

**Methods to pass the sudo passwords**

1. By using `--ask-become-password`
2. - store the password in a file 
   - pass the file by `--become-password-file=<file>`