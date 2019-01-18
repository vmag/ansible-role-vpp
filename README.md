Ansible role to deploy FD.IO VPP on Centos 7.

vpp adn honeycomb daemons are disabled, you need to create /etc/vpp/startup.conf and start vpp daemon:  

    systemctl enable vpp
    systemctl start vpp 
    
Optionally, you can start honeycomb:  

    systemctl start honeycomb
