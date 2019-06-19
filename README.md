# Prisma CloudFormation Templates 🚀

## Architecture 📐
![](./images/architecture.jpeg)

## Pre-requisites
- 🔑 **IAM Account** for *AWS CLI* (Requires pre-configuration using `aws configure`)
  ```bash
  $ aws configure
  ```
- Create service linked role
  ```bash
  $ aws iam create-service-linked-role --aws-service-name ecs.amazonaws.com
  ```

## Download CloudFormation Templates 📄
- `prisma.mysql.yml`
  - MySQL Template
  - [Download](/prisma.mysql.yml)
- `prisma.aurora.serverless.yml`
  - Aurora Serverless Template
  - [Download](/prisma.aurora.serverless.yml)

## How to deploy
- Download the template file for your desired DB below
- Go to [AWS CloudFormation Console](https://ap-northeast-2.console.aws.amazon.com/cloudformation)
- Click `Create Stack`
![](./images/screenshot-1.png)
- Check `Upload a template file`
- Click `Choose File` and choose template file (`.yml`)
- Click `Next`
![](./images/screenshot-2.png)
- Enter `Stack Name`
- Modify specific details
- Click `Next`
![](./images/screenshot-3.png)
- Click `Next`
![](./images/screenshot-4.png)
![](./images/screenshot-5.png)
- Check `I acknowledge that AWS CloudFormation might create IAM resources.`
- Click `Create Stack`
![](./images/screenshot-6.png)
- When the deployment ended, you can find an endpoint of prisma in `Outputs` section.

## Todos
- [ ] PostgreSQL Template
- [ ] MongoDB(DocumentDB) Template
