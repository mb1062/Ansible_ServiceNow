
# Ansible_ServiceNow

#Playbooks

This repository will include playbooks for Ansible and Service Now Integration

You can find here playbooks to:

        - Create a reccord on ServiceNow
        - Update a reccord on ServiceNow
        - Delete a reccord on ServiceNow

#Arguments

These playbooks use differents arguments,
There is two type of variable, secured by vault (args.yml) and not secured (params.yml)
Below a list of parameters common to these playbboks
For args.yml:

        - company       ->      The name of the company
        - api_username  ->      Username of the ServiceNow server account
        - api_password  ->      Password of the ServiceNow server account

For params.yml:

        - vm_name               ->      Name of the VM
        - snow_inst             ->      Address or DNS name of the ServiceNom server
        - table_name            ->      Name of the table in ServiceNow cmdb
        - os_inst               ->      Operating system of the VM
        - short_description     ->      Short description about the VM
        - install_status_inst   ->      Installed Status
        - sys_id                ->      Id of the reccord


