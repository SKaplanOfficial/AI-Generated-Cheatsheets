# AWS Cheatsheet

Amazon Web Services (AWS) is a cloud computing platform that provides a wide range of services and tools for building and deploying applications. Here is an overview of some of its basic syntax and features.

## EC2

### Launching an instance
```
aws ec2 run-instances --image-id ami-0c55b159cbfafe1f0 --count 1 --instance-type t2.micro --key-name my-key-pair --security-group-ids sg-1234567890abcdef0
```

### Stopping an instance
```
aws ec2 stop-instances --instance-ids i-1234567890abcdef0
```

### Starting an instance
```
aws ec2 start-instances --instance-ids i-1234567890abcdef0
```

## S3

### Creating a bucket
```
aws s3 mb s3://my-bucket-name
```

### Uploading a file
```
aws s3 cp /path/to/local/file s3://my-bucket-name/path/to/s3/file
```

### Downloading a file
```
aws s3 cp s3://my-bucket-name/path/to/s3/file /path/to/local/file
```

## Lambda

### Creating a function
```
aws lambda create-function --function-name my-function --runtime python3.8 --role arn:aws:iam::123456789012:role/lambda-role --handler lambda_function.lambda_handler --zip-file fileb://function.zip
```

### Invoking a function
```
aws lambda invoke --function-name my-function --payload '{"key1": "value1", "key2": "value2", "key3": "value3"}' output.txt
```

## Resources

- [AWS Documentation](https://docs.aws.amazon.com/index.html)
- [AWS CLI Command Reference](https://docs.aws.amazon.com/cli/index.html)