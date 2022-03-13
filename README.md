# terraform_kms

Terraform module to create KMS encryption keys.

## Variables

``` terraform
description: Description to understand what key is used for what service
organization: Allow root user to use KMS key
region: Region in which the key should be created
```

## Terraform example

``` terraform
######################
# KMS
######################
module "kms-cloudwatch" {
  source = "github.com/virsas/terraform_acm"
  description = "KMS key for Cloudwatch"
  region = "eu-west-1"
  organization = 012345678901
}
```
