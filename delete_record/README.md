
# Ansible_ServiceNow

# Playbooks

This repository will include the playbooks Ansible for deleting a reccord and his parameters file

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
        - sys_id                ->      Id of the reccord on ServiceNow
# Run

To run the playbook:

Use the command ansble-playbook with the location of the playbook as argument
You can overload a Parameter with the option -e and the define the new parameter parameter=myparameter

# Example

With parameters configured with files
#ansible-playbook deletereccord.yml 

With parameters overloaded
#ansible-playbook deletereccord.yml -e sys_id=123456789123456789


