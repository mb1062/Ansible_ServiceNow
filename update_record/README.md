
# Ansible_ServiceNow

# Playbooks

This repository will include the playbooks Ansible for updating a reccord and his parameters file

To update a reccord you should configure again the differents parameters, and they will be overwrite 

You can change the parameters below

	- vm_name
	- company
	- install_status_inst
	- short_description

You can find here:

        - The playbook createreccord.yml
        - The parameters file params.yml
        - The secure parameters file args.yml



Below the list of common parameters that you have to define for this playbook

args.yml:

        - api_username          ->      Username of the ServiceNow server account
        - api_password          ->      Password of the ServiceNow server account

For params.yml:

        - snow_inst             ->      Address or DNS name of the ServiceNom server
        - table_name            ->      Name of the table in ServiceNow cmdb
        - vm_name               ->      Name of the Virtual Machine which has just been created
        - company               ->      Name of the company which own the Virtual Machine
        - install_status_inst   ->      Status of the Virtual Machine installation
        - short_description     ->      A short description of the Virtual Machine
        - os_inst               ->      The name of the OS, the field should be define with the list of OS available

# Run

To run the playbook:

Use the command ansble-playbook with the location of the playbook as argument
You can overload a Parameter with the option -e and the define the new parameter parameter=myparameter

# Example

With parameters configured with files
#ansible-playbook updatereccord.yml 

With parameters overloaded
#ansible-playbook updatereccord.yml -e company=mycompany

