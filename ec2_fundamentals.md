# EC2 Fundamentals

## 1. Why does Amazon EC2 stand for Elastic Compute Cloud?

Amazon EC2 stands for Elastic Compute Cloud because it gives users virtual servers in the cloud that can be scaled up or down based on demand. The word elastic means the resources can grow when more computing power is needed and shrink when demand goes down.

## 2. Four essential infrastructure features provided by EC2

EC2 provides virtual machines, storage, networking, and load balancing. These are considered Infrastructure as a Service because AWS provides the core infrastructure, while the user controls the operating system, software, and applications.

## 3. EC2 billing model

EC2 uses a pay-as-you-go billing model. This means users only pay for the resources they use. When instances are scaled down or shut down, the cost decreases because fewer resources are running.

## User Data

### 1. What is the process of bundling configuration commands into a script called?

This process is called bootstrapping.

### 2. Under which user profile are User Data scripts executed?

User Data scripts are executed as the root user.

### 3. How many times does a User Data script run?

A User Data script runs one time during the first boot of the EC2 instance.
