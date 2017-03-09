ansible-role-ssh_config
===========================

Generate a ~/.ssh/config with your inventory (keep your old .ssh/config in backup)

Playbook example : ( file local_ssh_config.yml )
```
  ---
   - hosts: all
     become: no
     gather_facts: yes

   - hosts: localhost
     connection: local
     become: false
     roles:
      - ssh-config
```
