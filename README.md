# PRJ_Cloud
### Efrei Paris M1 SE1 Students: FENG & FOUR
cf. : Requirements: https://github.com/pascalito007/efrei-cloud-bigdata/tree/master/capstone-project

# I. App deployment




# II. 10 Quiz
## 1. Iam Quiz
1. Which statement describes AWS Identity and Access Management (IAM) users ?

-   Option 1. IAM users are used to control access to a specific AWS resource
-   Option 2. IAM users are used to control access to a specific AWS resource
-   Option 3. Every IAM user for an account mush have a unique name
-   Option 4. Every IAM user name is unique across all AWS accounts

        Option 1 


2. How can you grant the same level of permissions to multiple users within an account?

Option 1. Apply an AWS Identity and Access Management (IAM) policy to an IAM group

Option 2. Apply an AWS Identity and Access Management (IAM) policy to an IAM role

Option 3. Create a resource-based policy

Option 4. Create an organization in AWS Organizations


3. Which statements describe AWS Identity and Access Management (IAM) roles? (Select TWO.)

Option 1. They are uniquely associated to an individual

Option 2. They can only be used by accounts associated to the person who creates the role

Option 3. They can be assumed by individuals, applications, and services

Option 4. They provide temporary security credentials

Option 5. They provide permanent security credentials


4. Which statement describes a resource-based policy

Option 1. It can be applied to any AWS resource

Option 2. It can be an AWS managed policy

Option 3. It is attached to a user or a group

Option 4. It is always an inline policy


5. How does AWS Identity and Access Management (IAM) evaluate a policy?

Option 1. It checks for explicit allow statements before it checks for explicit deny statements

Option 2. It checks for explicit deny statements before it checks for explicit allow statements

Option 3. If there is no explicit deny statement or explicit allow statement, users will have access by default

Option 4. An explicit deny statement does not override an explicit allow statement


6. A team of developers needs access to several services and resources in a virtual private cloud (VPC) for 9 months. How can you use AWS Identity and Access Management (IAM) to enable access for them?

Option 1. Create a single IAM user to the developer team and attach the required IAM policies

Option 2. Create an IAM user for each developer, and attach the required IAM policies to each IAM user

Option 3. Create an IAM user for each developer, put them all in an IAM group, and attach the required IAM policies to the IAM group

Option 4. Create a single IAM user for the developer team, place it in an IAM group, and attach the required IAM policies to the IAM group


7. How does identity federation increase security for an application that it built in Amazon Web Services (AWS)?

Option 1. Users can use single sign-on (SSO) to access the application through an existing authenticated identity

Option 2. The application can synchronize user's user names and passwords in AWS identity and Access Management (IAM) with their social media accounts

Option 3. The browser can establish a trust relationship with the application to bypass the need for multi-factor authentication (MFA)

Option 4. Users can use their AWS Identity and Access Management (IAM) accounts to log in to on-premises systems


## 2. Network Quiz
1. Which definition describes a virtual private cloud (VPC)?

Option 1. A virtual private network (VPN) in the AWS Cloud

Option 2. An extension of an on-premises network into Amazon Web Services (AWS)

Option 3. A logically isolated virtual network that you define in the AWS Cloud

Option 4. A fully managed service that extends the AWS Cloud to customer premises


2. A company's VPC has the CIDR block 172.16.0.0/21 (2048 addresses). It has two subnets (A and B). Each subnet mush support 100 usable addresses now, but this number is expected to rise to at most 254 usable addresses soon. Which subnet addressing scheme meets the requirements and follows AWS best practices?

Option 1. Subnet A: 172.16.0.0/25 (128 addresses) Subnet B: 172.16.0.128/25 (1024 addresses)

Option 2. Subnet A: 172.16.0.0/25 (128 addresses) Subnet B: 172.16.0.128/25 (128 addresses)

Option 3. Subnet A: 172.16.0.0/23 (512 addresses) Subnet B: 172.16.0.128/23 (512 addresses)

Option 4. Subnet A: 172.16.0.0/22 (1024 addresses) Subnet B: 172.16.0.128/22 (128 addresses)


3. Which combination of actions enables direct internet access for IPv4 hosts in a virtual private cloud (VPC)? (Select THREE.)

Option 1. Creating a route for 0.0.0.0/0 that points to the internet gateway

Option 2. Enabling Domain Name System (DNS) resolution for the VPC

Option 3. Configuring hosts to have or obtain an internet-routable address

Option 4. Configuring the VPC domain name in a Dynamic Host Configuration Protocol (DHCP) options set

Option 5. Creating a default route that points to the virtual private gateway

Option 6. Configuring security groups and network access control lists (network ACLs) to permit internet traffic


4. Several EC2 instances launch in a virtual private cloud (VPC) that has internet access. These instances should not be accessible from the internet, but they must be able to download updates from the internet. How should the instances launch?

Option 1. With Elastic IP addresses, in a subnet with a default route to an internet gateway

Option 2. With public IP addresses, in a subnet with a default route to an internet gateway

Option 3. Without public IP addresses, in a subnet with a default route to an internet gateway

Option 4. Without public IP addresses, in a subnet with a default route to a network address translation (NAT) gateway




# III. IAM
1. 
```{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "AllowEC2AndS3",
      "Effect": "Allow",
      "Action": [
        "ec2:RunInstances",
        "ec2:TerminateInstances",
        "s3:GetObject",
        "s3:PutObject"
      ],
      "Resource": [
        "arn:aws:ec2:us-east-1:123456789012:instance/*",
        "arn:aws:s3:::example-bucket/*"
      ]
    }
  ]
}
```

Question: What actions are allowed for EC2 instances and S3 objects based on this policy? What specific resources are included?




# IV. AWS Quicksight


