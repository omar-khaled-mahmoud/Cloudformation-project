# Cloudformation-project

In this project , we will install apache server on EC2 inside private subnets having autoscalling group policy, the EC2 servers will communicate with an S3 bucket to copy the apache web server files from a persistent storage , and will  configure 4 subnets , 2 private and 2 public subnets, the public subnet will be attached to a load balancer and an autoscalling group , the private subnets will reach the internet via NAT gate ways deployed in the public subnet.

--for the EC2 to call the s3 bucket, it will need credentials, a new role is created and attached to the EC2 servers ( IamInstanceProfile: To-allow-ec2-call-s3-bucket )
