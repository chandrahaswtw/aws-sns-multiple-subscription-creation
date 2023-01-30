# SNS Multiple subscription creation

This repository explains how to add multiple subscriptions (email end-points in this case) using serverless and cloudformation templates.

## INSTALLATION
```
npm install
```

## USAGE
Add the emails in .env file with comma seperated. Example emails are mentioned in the .env file.

## IAM ROLE
As mentioned in the sns.yml file, we are using a pre-defined role for the lambda which give the permissions to add multiple email end points to an SNS topic. The role **lambda-sns.json** is attached on roles folder for your reference.

## DEPLOYMENT

```
serverless deploy --stage dev
```
Here **dev** being the example stage.

## RESULT
Once deployed successfully, you should see multiple email endpoints to the SNS Topic.