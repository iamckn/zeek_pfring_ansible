# zeek_pfring_ansible
Ansible playbook for the installation of pf_ring and zeek

# On the client

```bash
git clone https://github.com/iamckn/zeek_pfring_ansible
cd zeek_pfring_ansible
```

Edit the hosts file in that folder and fill in the IP field with the zeek server IP

# Prerequisites

```bash
ansible-playbook setup.yml -u root -k -i hosts -t pre_setup
```

# Install pf_ring

```bash
ansible-playbook setup.yml -u root -k -i hosts -t install_pf_ring
```

# Install zeek

```bash
ansible-playbook setup.yml -u root -k -i hosts -t install_zeek
```

# Install filebeat

```bash
ansible-playbook setup.yml -u root -k -i hosts -t install_filebeat
```

# Install Everything

```bash
ansible-playbook setup.yml -u root -k -i hosts
```
