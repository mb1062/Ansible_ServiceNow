
# Ansible_ServiceNow

# Playbooks

This repository will include playbooks for Ansible and Service Now Integration

You can find here playbooks to:

        - Create a reccord on ServiceNow
        - Update a reccord on ServiceNow
        - Delete a reccord on ServiceNow

# Arguments

These playbooks use differents arguments,
There is two type of variable, secured by vault (args.yml) and not secured (params.yml)


Below the list of common parameters that you have to define for each playbook

args.yml:

        - api_username  ->      Username of the ServiceNow server account
        - api_password  ->      Password of the ServiceNow server account

For params.yml:

        - snow_inst     ->      Address or DNS name of the ServiceNom server
        - table_name    ->      Name of the table in ServiceNow cmdb

# Run

To run a playbook:

Use the command ansble-playbook with the location of the playbook as argument
You can overload a Parameter with the option -e and the define the new parameter parameter=myparameter

# Example

With parameters configured with files
#ansible-playbook createrecord.yml 

With parameters overloaded
#ansible-playbook createrecord.yml -e sys_id=123456789123456789

# OS

Below the list of OS available for the parameter os_inst
The paremeter should be write exaclty with the same string

list of OS:

- Linux RedHat
