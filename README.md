# ansible-consul-demo
Demo of Consul and Ansible

## Installation

1. Spin-up some Ubuntu servers on AWS (or any other hosting)
1. Edit the IPs of the servrs in the provided `hosts` file (present at the 
same level as this README)
1. Create `ssh` folder under this checkout (same level as README)
1. Save a private SSH key under the ssh/private-key.pem
1. Make sure your private key permissions are valid:
  
       chmod 700 ssh
       chmod 600 ssh/*

## Quickstart

To make sure your SSH/AWS setup is functional, create `ssh` folder in the
ansible-consul-demo checkout

To make sure your ssh and hosts setup is correct and you can login to all 
required servers:

```console
ansible -i hosts all -m ping
```