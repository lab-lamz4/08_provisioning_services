# 08_provisioning_services

The task is to create an infrastructure via CloudFormation.

## Folder 01_CF

Folder 01_CF is an example to create a single EC2 instance and provision http web server using UserData. File 08-01-changeset.yml contains a fix in SecurityGroup that allows incoming traffic into EC2 instance.

## Folder 02_CF

Folder 02_CF is an example to create:
VPC
Security Groups that allow traffic into the appropriate destination
Internet GW
2 public Subnet
NAT GW 
2 private Subnet 
Routing
Ec2 - bastion + provision a user via UserData and Cloud-init
Ec2 - two web servers that serve as targets for Target Group, provision via UserData and Cloud-init
Load Balancer + TG + Listener
After creation, we got links in output to check that our ALB works correctly and we should see a web page that contains the hostname of each of the hosts.
