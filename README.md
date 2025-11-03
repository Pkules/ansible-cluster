# ansible-cluster
ansible cluster for CPU mining 
Setup:
add your miners in hosts file, -  setup ssh keys so you dont need login


Playbooks:
Create playbooks to run on miners

Run:

ansible-playbook -i ~/ansible-cluster/hosts.yml Working_install_Minerd_icminers.yml --ask-become-pass

run "ansible-playbook -i ~/hosts.ymlfilepath Someplaybookyoucreated.yml -- ask for sudo password^^ 
