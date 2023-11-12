# Ansible - Playbook

### Playbook to update the ubuntu servers
<br>

To run the playbook
```bash
ansible-navigator run -m stdout update_ubuntu_servers.yml --ask-become-password
```
```bash
ansible-playbook update_ubuntu_servers.yml --ask-become-password
```
<br>

**Important things to note !!**

1. username = ansible (change if you insist)
2. Playook works only with the **Debian** or **Ubuntu** with apt 


<br>

**Methods to pass the sudo passwords**

1. By using `--ask-become-password`
2. - store the password in a file 
   - pass the file by `--become-password-file=<file>`