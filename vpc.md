## Introduction to VPC (Virtual Private Cloud)
> A Private network to deploy your resources.
> Inside VPC we have `subnets` which allows partition of network. 
> They are defined at `Availability Zone level`.

![VPC](images/vpc/vpc-subnets.png)


> `A Public Subnet:` Is Accessible from the internet while `private subnet` not accessible from the internet.
>
>To define access to the internet and between subnets, we use `Route Tables` which defines how network flows between subnets. 

> VPC has set of IP range known as `CIDR` range i.e ranges of IP addresses allowed within your VPC.

## Internet Gateway
> What makes the subnet public and how can it access the internet ? We use `Internet Gateway` which helps VPC instances connect to the internet. 
>
>Public subnet will have a route to the Internet Gateway, thus making it public. 

![AWS VPC](images/vpc/aws-vpc.png)

>Suppose we have an EC2 Instance in the Private subnet & we want it to access the internet, i.e to get updates for softwares etc, but we do not want it to be accessible from the internet, we use a `NAT Gateway`.
>NAT Gateway(AWS Managed) & NAT Instance(Self Managed) allows your instance in your private subnet to access the internet while remaining private.

![NAT,IGW](images/vpc/vpc-nat-igw.png)

Private subnet can now access the internet through the NAT Gateway that connects to the Internet Gateway.

## Network ACL & Security Group
**[Network ACL](https://docs.aws.amazon.com/vpc/latest/userguide/vpc-network-acls.html):** A firewall that controls traffic from and to a subnet. Can have ALLOW & DENY rule.
- Attached at the subnet level.
- Rules only include IP Addresses.

## Security Group
A firewall that controls traffic to & from an ENI or an EC2 Instance.
- Can only have ALLOW rule.
- Rules include IP Addresses and other Security Group.

## Security Group VS Network Access Control List(NACL)

| Security Group    | Network Access Control List (NACL)    |
|:-----------------  |                 :----------          |
|Operates at Instance level | Operate at Subnet Level       |
|Support Allow rule only | Support both ALLOW & DENY rule   |
|Stateful: Return traffic is automatically allowed regardless of any rule. | Stateless: Return traffic MUST be EXPLICITLY allowed by rule.  |
| 