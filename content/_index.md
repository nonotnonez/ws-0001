---
title : " IaC with Terraform and AWS "
date : "`r Sys.Date()`"
weight : 1
chapter : false
---

# Infrastructure As Code with Terraform and AWS

#### Overview Project

In this workshop we will use **Terraform** interact with **AWS** to create
[VPC, Subnet](https://nonotnonez.github.io/ws-0001/3-tfconfig/3.1-vpcsubnet/),
EC2 , Route table, Internet gateway, Security group ...

#### Overview Terraform

Infrastructure as Code (IaC) tools allow you to manage infrastructure with configuration files rather than through a graphical user interface. IaC allows you to build, change, and manage your infrastructure in a safe, consistent, and repeatable way by defining resource configurations that you can version, reuse, and share.

Terraform plugins called providers let Terraform interact with cloud platforms and other services via their application programming interfaces (APIs). HashiCorp and the Terraform community have written over 1,000 providers to manage resources on Amazon Web Services (AWS), Azure, Google Cloud Platform (GCP)...

![0](/ws-0001/images/1/tf-hashicorp.png?featherlight=false&width=50pc)

#### Content

1. [Introduction](/ws-0001/1-intro/)
2. [Prepairation](/ws-0001/2-prepair/)
3. [Terraform Configure](/ws-0001/3-tfconfig/)
4. [Resource Cleanup](/ws-0001/4-cleanup/)