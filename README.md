# CodeForge-AD
This is the official powershell script for Codeforge Innovations AD seup.


# Overview
The CodeForge Active Directory Setup Script is a PowerShell automation script used to deploy and configure CodeForge’s Windows Active Directory environment in a consistent and repeatable manner.

The script is designed to streamline the provisioning of a Domain Controller and associated domain-joined workstations, ensuring that identity services, domain policies, and system configurations are applied uniformly across the environment. This supports both operational readiness and controlled security testing activities.

# What the Script Does
The script automates key Active Directory setup tasks, including:

- Domain Controller configuration and promotion

- Active Directory domain creation (codeforge.local)

- DNS and identity service initialization

- Domain join operations for Windows workstations

- User, group, and policy configuration required for daily operations

- Standardized system configuration to reduce setup inconsistencies

By using automation, CodeForge ensures faster deployments, reduced human error, and consistent environments across development, testing, and training use cases.

# How the Script Is Used
The script is executed locally on each Windows system involved in the deployment:

- On the Windows Server, the script initializes and configures the Domain Controller.

- On Windows workstations, the script joins systems to the CodeForge domain and applies required configurations.

The script follows a guided execution flow, prompting the operator to run specific setup steps in sequence. Reboots may be required between stages to complete system-level changes.

Execution is intended to be performed in a controlled virtualized environment and should follow CodeForge’s internal setup documentation or video guides where provided.

# Intended Use
This script is intended for:

- Standardizing CodeForge’s Active Directory deployments

- Supporting internal development and testing environments

- Enabling structured, authorized security assessments

- Training and onboarding technical staff in a controlled setting

It is not intended for public or unauthorized deployment.

# Notes

- The script should be run with Administrator privileges.

- Systems must meet the required Windows version and networking prerequisites before execution.

- All deployments should follow CodeForge’s internal rules of engagement and change-control processes.
