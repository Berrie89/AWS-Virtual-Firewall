# AWS-Virtual-Firewall
## Security Group
A security group is a virtual firewall that controls traffic to and from an instance. Security groups are stateful which means all inbound traffic are allowed to flow out regardless of outbound rules. Security groups use a default deny approach, it denies all traffic that is not explicitely allowed by a rule. When you create a security group you must create inbound rules to allow traffic into your instance.
### Setting up Security Group
i. I navigated to the security group section on the AWS console.
I 

## Network Access Control List (NACL)
NACL is a virtual firewall that controls traffic in and out of your subnets. Your Virtual Private Cloud (VPC) comes with a default NACL which by default allows all inbound and outbound traffic. You can create a custom NACL which by default denies all inbound and outbound traffic until you add rules. Each subnet in your VPC must be associated with a NACL. If you don't explicitely associate a subnet with a NACL, the subnet is automatically associated with the default NACL. NACLs contain a numbered list of rules that are evaluated in order, starting with the lowest numbered rule. NACLs are stateless which means they have seperate inbound and outbound rules and each rule can either allow or deny traffic.
### Setting up of NACL
