Create and upload these 3 files to S3:
iam-template.yaml
lambda-template.yaml
ssm-template.yaml

Replace https://s3.amazonaws.com/YOUR_BUCKET/... with the actual S3 URLs in the parent template.
Ensure each child template defines appropriate Outputs:
RegisterLambdaRoleArn and AutomationRoleArn from IAMStack
Lambda and SSM resources using those roles

Deploy root-template.yaml using CloudFormation.
