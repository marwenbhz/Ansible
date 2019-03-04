# How to install Ansible on Ubuntu Server.
  
  1* Update && upgrade
  sudo apt-get update
  sudo apt-get upgrade -y
  
  2* Install Ansible
  sudo apt-add-repository ppa:ansible/ansible
  sudo apt-get update
  sudo apt-get install ansible -y
  
  3* Configure SSH access to the server
  ssh-keygen
  cat ~/.ssh/id_rsa.pub
  ssh-copy-id NODE_IP
  
  4* Setting up our node
  
  5* Test
  ansible -m ping all
     Result:
              3.209.38.194 | SUCCESS => {
                  "changed": false, 
                  "ping": "pong"
              }
              3.208.43.200 | SUCCESS => {
                  "changed": false, 
                  "ping": "pong"
              }

  
