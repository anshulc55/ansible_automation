# Ansible Automation

Welcome to the Ansible Automation repository! This project contains various Ansible playbooks and roles designed to automate infrastructure management tasks. The goal is to provide a robust and reusable set of Ansible scripts to help streamline and standardize deployment and configuration processes.

## Table of Contents

- [Getting Started](#getting-started)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Getting Started

To get started with this project, clone the repository to your local machine and follow the instructions below to set up and run the Ansible playbooks.

## Prerequisites

- Ansible 2.9 or higher
- Python 3.6 or higher
- SSH access to the target machines
- Necessary permissions on the target machines to perform the tasks defined in the playbooks

## Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/anshulc55/ansible_automation.git
   cd ansible_automation
   ```

2. **Install dependencies:**

   Ensure you have Ansible installed. If not, you can install it using pip:

   ```bash
   pip install ansible
   ```

## Usage

1. **Configure inventory:**

   Edit the `inventory.ini` file to define your target hosts and groups.

   ```ini
   [webservers]
   webserver1 ansible_host=192.168.1.10 ansible_user=your_username

   [dbservers]
   dbserver1 ansible_host=192.168.1.20 ansible_user=your_username
   ```

2. **Run a playbook:**

   Use the `ansible-playbook` command to run a specific playbook. For example, to run the `site.yml` playbook:

   ```bash
   ansible-playbook -i inventory.ini site.yml
   ```

## Project Structure

The project is structured as follows:

```
ansible_automation/
├── ansible.cfg          # Ansible configuration file
├── inventory.ini        # Inventory file for defining target hosts
├── playbooks/           # Directory containing Ansible playbooks
│   ├── site.yml         # Main playbook to run
│   ├── webserver.yml    # Playbook for setting up web servers
│   └── dbserver.yml     # Playbook for setting up database servers
├── roles/               # Directory containing Ansible roles
│   ├── common/          # Common tasks for all servers
│   ├── webserver/       # Tasks specific to web servers
│   └── dbserver/        # Tasks specific to database servers
└── README.md            # This README file
```

## Contributing

Contributions are welcome! If you find a bug or have a feature request, please open an issue. If you would like to contribute code, please fork the repository and submit a pull request.

1. **Fork the repository**
2. **Create a new branch** (`git checkout -b feature-branch`)
3. **Commit your changes** (`git commit -am 'Add new feature'`)
4. **Push to the branch** (`git push origin feature-branch`)
5. **Open a pull request**

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For any questions or inquiries, please contact Anshul Chauhan at anshulc55@gmail.com.

---

Thank you for using Ansible Automation! Happy automating!
