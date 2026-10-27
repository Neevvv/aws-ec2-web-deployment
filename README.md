# AWS EC2 Web Application Deployment

## Project Overview
Deployed a static portfolio website on an Amazon EC2 Linux instance using Apache HTTP Server. Configured network access through an EC2 security group and monitored instance health and performance using Amazon CloudWatch.

## AWS Services Used
- Amazon EC2 — virtual server hosting the website
- Amazon VPC — networking for the instance
- EC2 Security Groups — inbound traffic control
- Amazon CloudWatch — performance metrics and CPU alarm

## Architecture
User's Browser → Internet → EC2 Security Group → EC2 Instance → Apache Web Server → HTML/CSS Website

CloudWatch collects EC2 performance metrics and evaluates the CPU alarm.

## Implementation Steps
1. Launched a Linux EC2 instance.
2. Configured inbound security group rules for HTTP and restricted SSH.
3. Installed and started Apache.
4. Created and deployed the portfolio webpage.
5. Verified the website using the instance's public IPv4 address.
6. Viewed EC2 metrics in CloudWatch and configured a CPU utilization alarm.

## Security Measures
- Restricted SSH access to my IP address.
- Allowed public HTTP traffic for website access.
- Used a dedicated security group for the application.
- Avoided storing private keys or credentials in the repository.

## Testing and Evidence
Add screenshots of:
- EC2 instance running
- Security group inbound rules
- Website open in a browser
- CloudWatch alarm configuration and status

## Outcome
Successfully deployed a web application on EC2, configured network security, and set up basic cloud monitoring.

## Future Improvements
- Configure HTTPS with a valid TLS certificate.
- Add CloudWatch Agent for memory and disk metrics.
- Automate deployment with a script.
- Explore infrastructure automation using AWS CloudFormation.
