Docker Ansible Deployment
This repository contains an Ansible playbook (docker.yml) to deploy an Apache Docker container and configure networking for it. The playbook automates the process of setting up Docker, deploying the Apache service, and ensuring network accessibility.

Purpose
The purpose of this project is to demonstrate the deployment of Docker containers using Ansible, specifically focusing on deploying an Apache service within a Docker container and configuring its networking.

Requirements
To use this playbook, ensure you have the following prerequisites installed:

Docker installed on the target machine(s).
Ansible installed on the control machine.
Usage
Clone the Repository:
git clone https://github.com/Eldhowilson14/Network_assignment.git

Navigate to the Repository:
cd docker-ansible-deployment

Update Inventory:
Update the Ansible inventory file (hosts) with your target machine(s) IP address(es).

Run the Playbook:
Execute the Ansible playbook using the following command:

ansible-playbook docker.yml

Verify Deployment:
Check if the Apache service is running in the Docker container.
Ensure accessibility to the Apache service from the host machine.
Playbook Structure
The docker.yml playbook is structured as follows:

Hosts Section: Specifies the target machine(s) where the tasks will be executed.
Tasks Section: Contains tasks for deploying the Apache Docker container and configuring networking.
Handlers Section: Handlers are triggered when notified by tasks. Currently not utilized in this playbook.
Network Configuration
The Apache Docker container is configured to run on the 172.168.10.0/30 subnet. The playbook ensures that the Apache service is accessible from the host machine.

Contributing
Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or create a pull request.

License
This project is licensed under the MIT License.
