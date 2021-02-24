## Run Cloudformation command:
### AWS Cloudformation create-stack
```
--stack-name vpc-cli
```
### Running vpc.yml
```
--template-body file://vpc.yaml
```
### AWS Cloudformation validate-template to create vpc
```
--template-body file://vpc.yaml
```
### AWS Cloudformation validate-template to create ec2
```
--template-body file://ec2.yaml
```
### AWS s3 copy index.html from s3 to suusarbucket
```
cp index.html s3://suusarbucket
```
### AWS s3 sync . s3://suusarbucket
```
s3 sync . s3://suusarbucket
```
### aws cloudformation update-stack
```
--stack-name vpc-cli
--template-body file://vpc.yaml
```
### run command command with params
```
aws cloudformation create-stack --stack-name startmyinstance
--template-body file://ec2.yaml
--parameters ParameterKey=SubnetType,ParameterValue=PublicSubnet
```