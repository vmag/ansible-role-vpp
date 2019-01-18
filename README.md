Ansible role to deploy FD.IO VPP v18.10 on Centos 7.
To run this role, you need to clone this repository to your Ansible roles folder and execute a playbook:

    ansible-playbook vpp.yaml

vpp and honeycomb daemons are disabled, you need to create /etc/vpp/startup.conf and start vpp daemon:  

    systemctl enable vpp
    systemctl start vpp 
    
Optionally, you can start honeycomb:  

    systemctl start honeycomb
