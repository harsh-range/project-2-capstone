# Static Website Hosting on Amazon S3 Using Terraform

## Overview

This project uses Terraform to deploy a simple static website on Amazon S3. The infrastructure is created as code, making it easy to provision and manage.

## Features

- Creates an Amazon S3 bucket
- Enables static website hosting
- Uploads an HTML file
- Makes the website publicly accessible

## Project Structure

```text
.
├── main.tf
├── terraform.tfvars
└── index.html
```

## Prerequisites

- AWS Account
- AWS CLI configured
- Terraform installed

## Deployment

Initialize Terraform:

```bash
terraform init
```

Review the execution plan:

```bash
terraform plan
```

Deploy the resources:

```bash
terraform apply -auto-approve
```

Get the website URL:

```bash
terraform output website_url
```

## Website Preview

The deployed website displays:

```text
Welcome to My Static Website!
Hosted on Amazon S3 using Terraform.
```

## Cleanup

To delete all created resources:

```bash
terraform destroy -auto-approve
```
