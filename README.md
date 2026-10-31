# AWS Lab 3.1 – Using Resource-Based Policies to Secure an S3 Bucket

**Author:** Salma Ben Hmida  
**Field:** Computer Science Engineering – Cybersecurity  
**Platform:** Amazon Web Services (AWS)  
**Project Type:** Hands-on Educational Security Lab

---

## 1. Project Overview

This project focuses on securing Amazon S3 resources using AWS Identity and Access Management (IAM) and resource-based policies.

The purpose of this lab was to understand how AWS controls access to cloud resources, how IAM roles interact with S3 bucket policies, and how permissions can be tested in different access scenarios.

Rather than simply configuring permissions, I explored how AWS evaluates access requests and how security policies can allow or deny specific actions.

## 2. Objectives

- Understand identity-based and resource-based policies.
- Explore IAM users and roles.
- Understand how role assumption works.
- Configure and examine S3 bucket access policies.
- Test authorized and unauthorized access.
- Understand the principle of least privilege.

## 3. AWS Services and Technologies

- Amazon S3
- AWS IAM
- S3 Bucket Policies
- IAM Roles
- AWS Management Console

## 4. Practical Work

During this lab, I worked with multiple S3 buckets and IAM roles to explore different access-control scenarios.

The practical exercises included:

- Examining IAM users and their permissions.
- Working with the `BucketsAccessRole` IAM role.
- Assuming an IAM role to access protected S3 resources.
- Examining S3 bucket policies and their permissions.
- Testing object access and upload operations.
- Comparing access results across different identities and roles.

## 5. Security Testing and Observations

The lab allowed me to observe how AWS evaluates access permissions in different scenarios.

Some key observations included:

- Direct access attempts by `devuser` were denied for protected S3 resources.
- Assuming `BucketsAccessRole` allowed access to a permitted object in another bucket.
- S3 bucket policies were used to define specific permissions, including object retrieval, object upload, and bucket listing.
- The `OtherBucketAccessRole` successfully uploaded an object to the designated third bucket, while other tested identities were denied access.

These tests demonstrated the importance of correctly configuring IAM permissions and resource-based policies.

## 6. Key Security Concepts Learned

**Identity-Based Policies:** Permissions attached to IAM identities, such as users and roles.

**Resource-Based Policies:** Policies attached directly to resources, such as S3 buckets.

**IAM Role Assumption:** Temporary access to AWS resources through an assumed role.

**Access Control:** Determining which identities can perform specific actions on cloud resources.

**Least Privilege Principle:** Granting only the permissions required to perform a task.

## 7. Key Takeaways

This lab helped me better understand how AWS access control works in practice.

It also reinforced the importance of testing permissions rather than assuming that a policy configuration automatically produces the intended security outcome.

I gained a better understanding of IAM role management, S3 bucket policies, access restrictions, and cloud security principles.

## 8. Disclaimer

This work was completed as part of an authorized educational AWS lab environment.

All activities were performed within the scope of the assigned exercises.

No production systems or unauthorized resources were tested.
