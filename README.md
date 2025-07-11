# Amazon Linux AMI Lab Documentation

This lab reinforced my knowledge of basic command line interface functionality and provided a foundation for learning more about Linux shell commands.

## Lab Objectives

- Used SSH to access an Amazon Linux AMI within Vocareum labs
- Learned the purpose of the `man` command
- Demonstrated the search feature of the man pages
- Examined man page headers

## Lab Components

The lab environment included:
- Amazon EC2 Command Host (in the public subnet)
- Public subnet
- Amazon Virtual Private Cloud (Amazon VPC)

## Step-by-Step Walkthrough

### Task 1: Connecting to Amazon Linux EC2 Instance via SSH

#### For Windows Users:
1. Downloaded the PPK file from Vocareum
2. Installed PuTTY (if not already installed)
3. Configured PuTTY with:
   - The public IP address provided
   - The downloaded PPK file for authentication
4. Established SSH connection to the EC2 instance

#### For Mac/Linux Users:
1. Used the terminal SSH command with the provided credentials
2. Connected to the instance using the public IP

### Task 2: Exploring Linux Man Pages

1. Accessed the manual pages for the `man` program itself:
   ```bash
   man man

## Key Learnings

1. **SSH Configuration**: Learned to set up SSH connections to EC2 instances using PuTTY
2. **Amazon Linux AMI**: Gained familiarity with the Amazon Linux environment
3. **Manual Pages**: Understood how to access and navigate Linux documentation
4. **Command Line Basics**: Reinforced fundamental CLI skills

## Next Steps

1. Explore more Linux commands and their man pages
2. Practice creating and managing EC2 instances
3. Learn about Amazon Linux 2023 (the newer version mentioned)
4. Experiment with other SSH clients and configurations


    ## SSH Connection Flow

```mermaid
sequenceDiagram
    participant User
    participant PuTTY
    participant EC2
    User->>PuTTY: 1. Download PPK
    User->>PuTTY: 2. Configure with IP/PPK
    PuTTY->>EC2: 3. Establish SSH Connection
    EC2-->>PuTTY: Authentication
    PuTTY-->>User: Connected to Amazon Linux
