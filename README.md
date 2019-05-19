

# AWS Challenges
AWS Challenges, originally written for Alten (Ctrl Alten Del) 1 day hackathon May 2019.  You will need a laptop for these challenges.  
Author: [Lim Chooi Guan](https://www.linkedin.com/in/cgl88/)

![AWS](https://australiancybersecuritymagazine.com.au/wp-content/uploads/2019/01/Amazon-Web-Services_logo835x396-702x336.png)

These challenges are created to allow you to learn and explore different capabilities of AWS.  There is no time limit for these challenges.

### Prerequisites
- AWS Account
- Working knowledge of AWS

### Challenge 1: Setting up a WordPress blog for your organization using Cloudformation, AMI and Auto scaling.
Scenario: You have been asked to set up a WordPress blog for your company to meet their defined specifications. During business hours (9 a.m.-6 p.m.), the blogging team would like to use their own development copy of the WordPress instance so that any changes don’t impact the live copy. 

Goals: Use Cloudformation to create an EC2 instance to run WordPress with the following specification:

- Instance Type: T2.micro
- Create a new AMI of the WordPress instance
- Configure Auto Scaling to launch a new WordPress instance

### Challenge 2:  Create an EC2 Linux instance for testing new applications

Scenario: The development team needs you to create a small Linux instance for testing a new application. You must create the EC2 instance per defined specifications. A few days later, the development team informs you that they want to move the instance into production, so they want you to change the specifications of the instance.

Goals: Create an EC2 instance with the following specifications:  
- AMI: Amazon Linux  
- Instance Type: T2.nano  
- Volume Type: 8GB Magnetic

Next, reconfigure the instance to achieve the following specification:  
- Instance Type: Scale to a T2.small  
- Volume Type: Increase to 12GB General Purpose SSD  
- Verify whether the root volume on the EC2 instance is displaying the correct size.

### Challenge 3: Distribute content using Cloudfront, S3, georestriction and enable logging

Scenario: Your company wants to distribute content in the form of a website to their global offices. Due to legal restrictions, you cannot distribute the content in France and Australia. You must find a way to prevent these offices from accessing the data. The content does not change very often; however, some of the files are very large, and you must find a solution to minimise end user latency. The last requirement is that the audit department wants to track those who access the website.

Goals of the project:  
- Set up a static website using Amazon S3.  
- Create a bucket and enable static website hosting.  
- Enable logging.  
- Set up a CloudFront distribution for the static website with Access Logs enabled.  
- Set up Geo Restrictions to prevent users in France and Australia from accessing the data.  
- Verify that logging is working.

### Challenge 4: Deploy a large Docker image in ECS

Scenario: Your company has a very large Docker image (> 10 gigabytes.  Note that you will have to create this image yourself, so spin up an nginx image and copy some large ISO files into this image in order to create a 'fake' large image) and want this to be deployed in an ECS cluster.  The Docker image has to be uploaded to ECR.  Your job is to deploy this image using ECS, ECR, and verify that the deployed container is working correctly.

Goals of the project:
- Create an ECS cluster.
- Create an ECR.
- Upload your large Docker image to ECR.
- Create a Task Definition comprising of a containier that loads this image.
- Verify that the container is working correctly.
