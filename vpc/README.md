Download the file and run

aws cloudformation create-stack \
--stack-name vpc-cli \
--template-body file://vpc.yaml

aws cloudformation validate-template \
--template-body file://vpc.yaml

aws cloudformation validate-template \
--template-body file://ec2.yaml


#aws s3 cp index.html s3://suusarbucket

#aws s3 sync . s3://suusarbucket





aws cloudformation update-stack \
--stack-name vpc-cli \
--template-body file://vpc.yaml

aws cloudformation create-stack --stack-name ec2 --template-body file://ec2.yaml


aws cloudformation update-stack \
--stack-name vpc-cli \
--template-body file://ec2.yaml

aws cloudformation update-stack \
--stack-name vpc-cli \
--template-body file://vpc.yaml

### run command command with params
aws cloudformation create-stack  --stack-name startmyinstance \
    --template-body file://ec2.yaml \
    --parameters  ParameterKey=SubnetType,ParameterValue=PublicSubnet