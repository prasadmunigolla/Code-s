# Create Lambda and DynamoDB using Cloud formation 

Follow below steps to setup environment. 
1. Create CloudFormation template using s3bucketcreation.yml  to create an S3 bucket 
2. Upload greeter.zip onto S3 bucket manually (We can automate this activaty too) 
3. Create another CloudFormation template using lambda-ddb-template.yaml. 

`s3bucketcreation.yml` - This creates a S3 bucket with the name blazeclan-lambda and add tags   
`lambda-ddb-template.yaml` - This is another template to create an DynamoDB, IAM Role, IAM Policy and Lambda function. Lambda function code (greeter.zip) reterived from S3 bucket   
`greeter.zip` - This is a boto3 script which stored in S3 bucket. This code helps to lambda to write on DynamoDB
