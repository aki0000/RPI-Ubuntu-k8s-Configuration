# RPI-Ubuntu-k8s-Configuration

### 1. Change Initial Password
ssh {user name}@{IP Address}

### 2. Register a Public key from Initial Server
ssh-copy-id -i ~/.ssh/id_rsa.pub {user name}@{IP Address}

### 3. Execute task
ansible-playbook -i hosts site.yaml -vvv --ask-become-pass --extra-vars="target_initial_address={} server_address={} gateway_address={}