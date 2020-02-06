# Linux automation using ansible


###Branch reset_to_factory_Dell_HP
The ansible playbook deals with resetting Dell idrac and HP ilo to factory settings.
Currently this playbook supports only CentOS machines.
Step 1: Modify host names mentioned in the inventory/hosts file.
Step 2: Run the command "ansible-playbook playbook/reset_ilo_idrac.yml -i inventory/hosts" with out quotes ofcourse.
Step 3: Now we wait for the HP ilo and Dell idrac to reset to factory settings.


####Branch reboot_and_wait_centos
The ansible playbook deals with rebooting a CentOS machine and waits for the host to be up.
Step 1: Modify host names in inventory/hosts file.
Step 2:  Run the command "ansible-playbook playbook/reboot.yml -i inventory/hosts" with out quotes ofcourse.
Step 3: Wait till the host gets up. If the playbook timed out then debug what happened to the host from the console.
