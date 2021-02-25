## Run Cloudformation command:
### creating aws cloudformation stack for vpc through aws cli
```
aws cloudformation create-stack --stack-name vpc-cli --template-body file://Documents/cfn/vpc.yaml
```

### creating stack for ec2 and through aws cli
```
aws cloudformation create-stack --stack-name ec2-cli --template-body file://Documents/cfn/ec2.yaml
```
### AWS s3 copy index.html from s3 to suusarbucket
```
cp index.html s3://suusarbucket
```
### AWS s3 sync . s3://suusarbucket
```
s3 sync . s3://suusarbucket
```
### run command with params
```
aws cloudformation create-stack --stack-name ec2-cli --template-body file://Documents/cfn/ec2.yaml --parameters ParameterKey=SubnetType,ParameterValue=PublicSubnet
```
