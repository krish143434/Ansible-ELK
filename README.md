# Ansible ELK Playbook
 
This playbook is for setting up version 7.x of the ELK Stack on a remote server. 

## Notes and requirements

 - The playbook was built and tested on Ubuntu 20 VMs, for ELK versions 7.x 
 - You will need Ansible installed and running
 - Playbook is currently configured to set up the ELK stack together with Metricbeat for server perf monitoring. There is a role for Filebeat as well. You just need to add the Filebeat role to your [site.yml] file.
 
 ## Instructions
 
 1. Add your IP of the host name under elkserver group within hosts file
 2. Verify connectivity to the ELK server.
 3. clone the repo
 4. Cd into the directory, and run:
 `ansible-playbook site.yml`
 
 The plays in the playbook will run on the target server, installing ELK and the specified beats shippers. 
 
