https://www.youtube.com/watch?v=UUkCys309xA

https://www.youtube.com/watch?v=oNK1fXhxQHs

# Vagrant and ansible:
https://devopsideas.com/ansible-local-setup-using-vagrant-virtualbox/

# Troubleshooting:
$ ip a 
$ yum install net-tools for getting ifconfig


# How to pass private key in ansible command:
~/tmp/vagrant/ansible-vagrant  vagrant ssh-config
--> /Users/a0k00ee/.vagrant.d/insecure_private_key

# Use the above in the ansible command:
ssh -i /Users/a0k00ee/.vagrant.d/insecure_private_key vagrant@192.168.33.10

http://docs.ansible.com/ansible/latest/intro_inventory.html

# Run the playbook:
ansible-playbook -i inventory site.yml -u vagrant | tee tomcat.md
