# Homelab Base

This repository provides a production-ready foundation for provisioning Ubuntu homelab servers using `cloud-init`, `ansible-pull`, and Docker. It aims to create a fully automated, idempotent, and modular system that can be easily extended.

## Features

- **Automated Provisioning**: From a fresh Ubuntu Server install, the system can be fully provisioned and configured with a single boot.
- **Idempotent Configuration**: Using Ansible, the configuration can be applied multiple times without changing the result.
- **Modular Design**: The system is broken down into Ansible roles, allowing for easy customization and extension.
- **Multiple Host Profiles**: Support for different server roles, such as an AI host, a VM host, or a full lab setup.
- **Docker and Docker Compose**: Easily run containerized applications.
- **KVM/libvirt**: Full virtualization support for running virtual machines.

## Getting Started

### Prerequisites

- A fresh installation of Ubuntu Server 22.04 LTS.
- A GitHub repository forked from this template.

### Initial Setup

1. **Fork this repository** to your own GitHub account.
2. **Customize the `cloud-init/user-data.example` file**:
   - Replace `your_username` with your desired username.
   - Replace the placeholder SSH key with your public SSH key.
   - Replace the GitHub repository URL with the URL of your forked repository.
3. **Provide the `user-data` file to your cloud instance** during creation. This will trigger the automated provisioning process.

For more detailed instructions, please refer to the documentation in the `docs` directory.

## Documentation

- [Architecture](docs/architecture.md)
- [Bootstrap Flow](docs/bootstrap-flow.md)
- [Cloud-Init Flow](docs/cloud-init-flow.md)
- [Windows 11 VM Setup](docs/windows11-vm.md)
- [Server Profiles](docs/server-profiles.md)

## Contributing

Contributions are welcome! Please feel free to open an issue or submit a pull request.
