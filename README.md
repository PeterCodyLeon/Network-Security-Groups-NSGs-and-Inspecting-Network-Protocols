![image](https://github.com/PeterCodyLeon/Network-Security-Groups-NSGs-and-Inspecting-Network-Protocols/assets/161895166/a5afe7de-9790-4a27-8f73-2ad17f08249f)




 Creating Network Security Groups NSGs and Inspecting Network Protocols
-----------


In AWS, security groups act as virtual firewalls for your Amazon EC2 instances to control inbound and outbound traffic. They are essentially sets of IP filter rules that control the traffic for one or more instances. Here's a breakdown of their key features and functionalities:


Inbound Rules: Security groups allow you to specify rules that control inbound traffic to your instances. For example, you can allow HTTP traffic (port 80) from any IP address or SSH traffic (port 22) from a specific IP range.


Outbound Rules: Similarly, you can configure outbound rules to control the traffic leaving your instances. By default, outbound traffic is allowed, but you can customize these rules to restrict outbound access if necessary.


Stateful: Security groups are stateful, meaning any traffic that's allowed in is automatically allowed back out. For instance, if you allow inbound traffic on port 80 for web servers, the response traffic from those web servers is automatically allowed back out.


Applied at Instance Level: Each instance in your VPC (Virtual Private Cloud) can be associated with one or more security groups. When you launch an instance, you can specify one or more security groups to be associated with it.


Changes in Real-time: Any changes made to security group rules take effect immediately. This means you can quickly update your security configurations in response to changing requirements or threats.


Implicit Deny: By default, security groups have an implicit "deny all" rule. This means that if you haven't explicitly allowed traffic, it's implicitly denied.
Flexible: Security groups are quite flexible and can be modified at any time. You can add or remove rules, change existing rules, and associate or disassociate them with instances as needed.


Layered Security: They are often used in conjunction with other AWS security measures such as Network Access Control Lists (NACLs) and AWS Identity and Access Management (IAM) to provide layered security.
