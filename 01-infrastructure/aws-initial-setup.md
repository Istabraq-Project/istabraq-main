# AWS Initial Setup Checklist

## 1. Services to Enable (Free Tier)
- [ ] EC2 (Elastic Compute Cloud) - for servers
- [ ] RDS (Relational Database Service) - PostgreSQL
- [ ] S3 (Simple Storage Service) - file storage
- [ ] Lambda - serverless functions
- [ ] CloudFront - CDN
- [ ] Route 53 - DNS (optional for now)
- [ ] IAM - identity management

## 2. Resource Limits (Free Tier)
- EC2: 750 hours/month of t2.micro/t3.micro
- RDS: 750 hours/month of db.t3.micro
- S3: 5GB standard storage
- Lambda: 1M requests/month
- CloudFront: 50GB data transfer/month

## 3. Estimated Monthly Cost: $0-$5
(If staying within free tier)

## 4. Security Groups to Create:
- web-access: HTTP/HTTPS access
- ssh-access: SSH for EC2 (restrict to your IP)
- db-access: PostgreSQL port 5432 (EC2 only)
- internal-only: For services talking to each other
