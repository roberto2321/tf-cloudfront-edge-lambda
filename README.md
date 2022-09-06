# tf-cloudfront-edge-lambda

CloudFront with Lambda@Edge using Terraform

## Overview

This repository contains the terraform files that creates an S3 bucket used to upload media and a CloudFront distribution to distribute that media through a Content Delivery Network. We also attach some Lambda@Edge on our CloudFront distribution to: Dinamically switch origins (in order to support image transformations using Cloudinary), unify the response provided from different origins, and require authentication in order to access the media.

In order to spin all the above, you will need:

- An AWS account
- A Cloudinary account
- Terraform installed

