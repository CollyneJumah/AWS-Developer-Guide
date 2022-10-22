# Introduction

>A physical server within a data center will be considered a compute resource as it may have multiple CPUs and many Gigabytes of RAM

>Compute services can comprise of utilizing hundreds of EC2 Instances(Virtual Servers) which may be used continuously for months or even years processing millions of istructions.

>Compute is closely related to common server components such as CPU & RAM

## Amazon EC2
EC2 Allows you to deploy virtual servers within your AWS environment
### Components of EC2
#### 1. Amazon Machine Images(AMI)
#### 2. Instance types
#### 3. Instance Purchasing Options
#### 4. Tenancy
#### 5. User Data
#### 6. Storage Options
#### 7. Security

### AMI
>>> They are essentially templates of pre-configured EC2 instances which allow you to quickly launch a new instance based on the configuration withinn the AMI.

>>An AMI is an image baseline with an operating system & applications along with any custom configuration.

#### Where to find AMI
- AWS Marketplace: An online store that allows you to purchase AMIs from trusted vendors.
- Community AMIs: Are repositories of AMIs that have been created and shared by other AWS member.

### Intance type:
> Once you've selected AMI from any of the different sources, you MUST select an instance type.
> It defines the size of instance based on the number of different parameters.  i.e ECU, vCPUS, Physical processor, amount of volume, network level status performance, Instance storage

| Instance Type     | Description
| :---              |:---
| Micro Instance    | Have a low cost instance option, providing low amount of CPU resources. Suitable for low throughput applications and websites that requires additional compute cycles periodically. Used for low traffic websites/ blogs, small administrative applications, bastian hosts |
| General Purpose   | Provides a balance of compute, memory and network|
| Compute Optimized |
| FPGA Instance     |
| GPU Instance      |
| Memory Optimized  |
| Storage Optimized |