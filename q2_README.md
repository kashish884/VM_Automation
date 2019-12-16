#Description
1. Playbook to create ovs network infra structure as shown in Assignment Q2.
2. Playbook to define network as internet (NAT/DHCP), l2 (bridge), l3 (routed), other (routed).
3. Playbook to create 2 VMs with 2 interfaces, 2 vcpu, 2 GB RAM, 12 GB disk space, and two applications, namely wireshark and iperf. VM1 should be connected to Internet and L2 Network. VM2 should be
connected to Internet and L2 Network.

#Usage
Provide the Guests (VM) requirements that you want to create inside guests_vars.yml and bridges requirements inside networks_vars.yml.
The q2.yml, networks_vars.yml, guests_vars.yml, bridge_template.xml.j2, vm_template.xml.j2 playbooks should be present in the ansible folder.

*run script with sudo command:
$ sudo ansible-playbook q2.yml 

Assumptions:
- Client has to set interface ip (which is connected with OVS bridge in routed mode)


*For bonus question:
The guests_vars_BONUS.yml file contents should be added in the guests_vars.yml file.


*virt-builder tool installation command:

sudo apt-get install libguestfs-tools

sudo chmod 0644 /boot/vmlinuz* 
[ to avoid occurence of libguestfs: error: /usr/bin/supermin exited with error status 1   error]




# Version
 - 1.0

#Authors
----
Kashish Singh, Sathwik Kalvakuntla

# License

  - All rights reserved by the owner and NC State University.
  - Usage of the code can be done post approval from the above.