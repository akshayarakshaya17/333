experiment 7 installation 
sudo apt update
sudo apt-get install software-properties-common
sudo apt-add-repostitory --yes--update ppa:ansible/ansible 
sudo apt-get install ansible 
   give yes 
ansible --version 



simple yml file for ansible 

- name: Description
  hosts: webservers
  become: true
  tasks:
    - name: Install Nginx
      apt:
        name: nginx
        state: present

