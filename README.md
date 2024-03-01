**Project: WordPress Website Hosting on AWS**

**Overview**: This project aims to deploy a WordPress website on Amazon Web Services (AWS) using various AWS services and best practices in DevOps. Below is a detailed guide on the architecture and deployment process.

**Deployment Steps:**

1. **Virtual Private Cloud (VPC)**:
   - Configured with public and private subnets across two availability zones for enhanced reliability and fault tolerance.

2. **Internet Gateway**:
   - Facilitates connectivity between VPC instances and the wider Internet.

3. **Security Groups**:
   - Acts as a network firewall mechanism to control traffic to EC2 instances.

4. **Availability Zones**:
   - Utilized to enhance system reliability and fault tolerance.

5. **EC2 Instances (Web Servers)**:
   - Deployed within private subnets for enhanced security.
   - Accessed via EC2 Instance Connect Endpoint for secure connection.

6. **NAT Gateway**:
   - Enables instances in private subnets to access the Internet.

7. **Application Load Balancer (ALB)**:
   - Distributes web traffic evenly to an Auto Scaling Group of EC2 instances across multiple availability zones.
   - Configured with a target group for routing traffic.

8. **Auto Scaling Group**:
   - Automatically manages EC2 instances to ensure website availability, scalability, fault tolerance, and elasticity.

9. **GitHub**:
   - Web files stored for version control and collaboration.

10. **Certificate Manager**:
    - Secures application communication using SSL/TLS certificates.

11. **Simple Notification Service (SNS)**:
    - Configured to alert about activities within the Auto Scaling Group.

12. **Route 53**:
    - Registered domain name and set up DNS records.

13. **RDS (Relational Database Service)**:
    - Deployed for database management.

14. **EFS (Elastic File System)**:
    - Deployed for scalable and elastic file storage.

15. **Bastion Host**:
    - Used to access the private network for application installation.

**Repository**: The reference diagram and deployment scripts for this project are available in the GitHub repository. Please refer to the repository for detailed instructions on deploying the static website on AWS infrastructure.

**Conclusion**: By following the instructions and utilizing the provided resources, you can successfully deploy a WordPress website on AWS, ensuring high availability, security, and scalability, database management, file storage.

