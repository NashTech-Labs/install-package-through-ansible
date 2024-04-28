# Running Ansible Playbook to Install a Python Package
 
This Ansible playbook is designed to install a Python package using the `pip` module on all hosts specified.
 
## Prerequisites
 
- Ansible installed on the machine from which you'll run the playbook.
- SSH access to the target hosts.
- Python installed on the target hosts (required for Ansible to execute tasks).
 
## Instructions
 
1. **Clone Repository**: Clone this repository to your local machine.
 
    ```bash
    git clone <repository-url>
    ```
 
2. **Navigate to Directory**: Navigate to the directory containing the playbook file (`install_package.yml`).
 
    ```bash
    cd <repository-directory>
    ```
 
3. **Update Inventory**: Ensure your inventory file (`hosts`) contains the target hosts where you want to install the Python package.
 
4. **Review Playbook**: Open the `install_package.yml` file and review the playbook to ensure it meets your requirements.
 
5. **Edit Playbook**: Update the playbook to specify the name of the Python package you want to install. Replace `<enter the package name>` with the name of the package you want to install.
 
6. **Run Playbook**: Execute the Ansible playbook using the `ansible-playbook` command, providing the playbook file and specifying any additional options as needed.
 
    ```bash
    ansible-playbook -i hosts install_package.yml
    ```
 
    Replace `hosts` with the path to your inventory file if it's located in a different directory.
 
7. **Verify Installation**: Once the playbook execution is complete, verify that the specified Python package is installed on the target hosts by logging into the hosts and checking for the package.
 
8. **(Optional) Customize**: If needed, customize the playbook or inventory file to add more tasks, target different hosts, or install additional packages.
 
## Notes
 
- Ensure that the SSH credentials provided in the inventory file have the necessary permissions to execute commands with elevated privileges (`sudo`) on the target hosts.

has context menu
