# Install LAMP and deploy a Demo Laravel Project with Ansible
## Also install and setup Postgresql

## Prerequisite

1. You'll need one Ubuntu 18.04 server to serve as node / host.
1. You'll need one Ubuntu server of your choice to serve as worker/control
2. Install Ansible
3. generate ssh keys and place your pub key on the Ansible worker ~/.ssh/auth 

## Steps to run Ansible set up

1. Clone this repository
2. Set up your inventory file
3. Adjust values on your `group_vars/all.yml` file
4. Run the `svr-setup.yaml` playbook to set up the LAMP server
5. Run the `laravel-deploy.yaml` playbook to deploy the demo Laravel application
6. Run the `run-postgress.yaml` playbook to install and setup Postgresql
7. Access your server's IP address or hostname to test the setup