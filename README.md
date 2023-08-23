# docker-compose.yml for ONLYOFFICE

## GitHub Repository: OnlyOffice and Traefik Setup with docker-compose

This repository provides a docker-compose configuration to set up OnlyOffice Document Server along with Traefik as a reverse proxy for secure access. By following the instructions below, you can quickly deploy the services while ensuring proper configuration for your environment.

### Prerequisites

Docker and Docker Compose are installed on your system.
You have a domain or subdomains that you intend to use for accessing OnlyOffice and Traefik.

### Getting Started

Clone this repository to your local machine:

```bash
git clone https://github.com/jschanz/docker_onlyoffice.git
cd docker_onlyoffice
```

### Configuration

#### docker-compose.yml

In the docker-compose.yml file, replace the following placeholders with appropriate values:

Replace __onlyoffice.domain.tld__ with your domain/subdomain for accessing OnlyOffice.

__JWT_SECRET__ - Set a secure JWT secret key. This can be any random string.

#### Deploy

Run the following command to start the services:

```bash
docker-compose up -d
```

This will pull and start the required container for OnlyOffice. The -d flag detaches the process, allowing the services to run in the background.

#### Access

OnlyOffice: Access the OnlyOffice Document Server using your configured domain in a web browser (e.g., <https://onlyoffice.domain.tld>).

#### Important Note

This docker-compose.yml requires a running Traefik installation. Remember to keep your configuration files and secrets secure. The JWT_SECRET should be a strong, random key for security reasons.

#### Troubleshooting

If you encounter any issues during the setup process, please refer to the official documentation for Docker, Docker Compose, OnlyOffice, and Traefik.

#### Contributions

Contributions to improve and expand this repository are welcome. Feel free to fork the repository, make your changes, and submit a pull request.

#### License

This project is licensed under the MIT License.

Disclaimer: This README is meant as a guide and might not cover all possible scenarios. Always refer to the official documentation of the tools and services used for more comprehensive instructions and troubleshooting.
