# Summary of App Deployment

## Architecture design diagram


## I. Setup AWS environment
1. Log in AWS account
2. Choose Paris as region

## II. Create a VPC
1. Create a new VPC
2. Fill in fields 
3. Mark down VPC ID

## III. Create a public and a private subnet
1. Create two subnets (public and private)
2. Fill in fields

## IV. Create an EC2 instance
1. Create an instance using Cloud9
2. Choose t2.micro and configure details (VPC and public subnet)
3. Configure SG to allow SSH (port 22) from my IP
4. Run the instance
5. Mark down instance ID

## V. Setup RDS instance
1. Create database
2. Select MySQL, use Free Tier, specifier DB instance identifier & master username & password
3. Choose VPC & private subnet
4. Enable VPC SG and configure inbound rule to allow traffic from EC2 instance
5. Give the database a name
6. Review everything and click "Create database"

## VI. Install and configure the PHP application
1. SSH into the EC2 instance 
2. Use the given script to install packages & website files & SQL file
3. Update PHP application with RDS endpoint and database credentials
4. Move the PHP application to the Apache directory 
5. Import SQL file to the RDS instance
6. Test application by using the previous EC2 public IP address 

## VII. Setup AWS Systems Manager Parameter Store
1. Go to Parameter Store
2. Create parameters with those given values

## VIII. Delete all used resources


## IX. Annex
Cf. : https://www.youtube.com/watch?v=aBgDXd_Brlw&ab_channel=DevOps%26CloudwithAryya 