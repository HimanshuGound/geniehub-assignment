## What Is AWS(Amazon Web Services)
->Amazon Web Services (AWS) is a comprehensive cloud computing platform offered by Amazon.com. It provides a wide range of cloud services, including computing power, storage options, networking, databases, machine learning, analytics, security, and more.

### Facility offer by AWS:
- Compute Services
- Storage Services
- Database Services
- Networking Services
- Analytics And Machine Learning
- Security and Identity Services
- Developer Tools
- Serverless Computing

### How to Create EC2 instance?
#### Sign in to the AWS Management Console:
   Go to the AWS Management Console (https://console.aws.amazon.com/) and sign in with your AWS account credentials.
#### Navigate to EC2 Dashboard:
Once logged in, navigate to the EC2 service by clicking on "Services" in the top left corner, then selecting "EC2" under the "Compute" section.   
#### Launch Instance: 
On the EC2 Dashboard, click on the "Launch Instance" button to start the process of creating a new EC2 instance.
#### Choose an Amazon Machine Image (AMI): 
Select an AMI that best fits your requirements. An AMI is a pre-configured template that contains the operating system and additional software needed to launch an instance. You can choose from AWS-provided AMIs, community AMIs, or your custom AMIs
#### Choose an Instance Type:
Select the instance type that suits your workload needs. Instance types vary in terms of CPU, memory, storage, and networking capacity. You can choose from a range of options, from general-purpose instances to compute-optimized, memory-optimized, and storage-optimized instances.
#### Configure Instance Details: 
Configure additional settings for your instance, such as the number of instances to launch, network settings (VPC, subnet, security groups), IAM role, monitoring options, and user data (optional scripts or commands to run when the instance starts).
#### Add Storage:
Specify the storage options for your instance. You can add additional volumes (EBS volumes) and configure their size, type (e.g., SSD, HDD), and encryption settings.
#### Add Tags (Optional): 
Add tags to your instance to help organize and manage your resources. Tags are key-value pairs that you can use to categorize instances and apply metadata.
#### Configure Security Group: 
Specify the security group settings for your instance. Security groups act as virtual firewalls, controlling inbound and outbound traffic to your instance. You can create a new security group or select an existing one.
#### Review and Launch: 
Review the configuration settings for your instance and make any necessary changes. Once you're satisfied with the configuration, click on the "Launch" button.
#### Create Key Pair: 
If you don't already have an existing key pair, you'll be prompted to create a new key pair. This key pair allows you to securely connect to your instance using SSH (for Linux instances) or RDP (for Windows instances).
#### Launch Instance: 
After creating or selecting a key pair, click on the "Launch Instances" button to launch your EC2 instance.
#### Access your Instance: 
Once the instance is launched, you can connect to it using SSH (for Linux instances) or RDP (for Windows instances) using the private key file associated with the key pair you selected.
