# Security Policies

## 1. Do security groups support both allow and deny rules?

No, security groups do not support both allow and deny rules. They only support allow rules. If traffic is not specifically allowed by a rule, it is blocked by default.

## 2. Default inbound and outbound traffic

By default, all inbound traffic is blocked. This means no outside traffic can reach the EC2 instance unless a rule allows it.

By default, outbound traffic is allowed if left unrestricted. This means the instance can send traffic out to other services or the internet.

## 3. Are EC2 instances aware of security groups?

EC2 instances are not internally aware of the security groups. Security groups are applied externally at the network level. One security group can also be reused across multiple EC2 instances.

## Core Port Mapping Matrix

| Port | Protocol | Purpose                                       |
| ---- | -------- | --------------------------------------------- |
| 22   | SSH      | Secure command-line access to a Linux server  |
| 21   | FTP      | File Transfer Protocol used to transfer files |
| 80   | HTTP     | Standard web traffic without encryption       |
| 443  | HTTPS    | Secure encrypted web traffic                  |
| 3389 | RDP      | Remote Desktop access for Windows servers     |
