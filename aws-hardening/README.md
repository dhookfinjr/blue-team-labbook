# AWS IAM Hardening & Misconfiguration Review

## 🔍 Overview
This project reviews AWS Identity & Access Management (IAM) policies and identifies misconfigurations that could lead to privilege escalation or account compromise. I created a checklist of best practices and documented a policy I reviewed and improved.

## ⚠️ Problem Policy (Too Permissive)
```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Effect": "Allow",
      "Action": "*",
      "Resource": "*"
    }
  ]
}
