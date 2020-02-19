# Infrastructure as Code

## Create Stack
```
aws cloudformation create-stack \
    --stack-name REDACTED \
    --parameters ParameterKey=EnvironmentName,ParameterValue=REDACTED_KEYVALUE \
    --parameters ParameterKey=VpcCIDR,ParameterValue=REDACTED_KEYVALUE \
    --parameters ParameterKey=Region,ParameterValue=REDACTED_KEYVALUE \
    --parameters ParameterKey=PublicSubnet1CIDR,ParameterValue=REDACTED_KEYVALUE \
    --parameters ParameterKey=PublicSubnet2CIDR,ParameterValue=REDACTED_KEYVALUE \
    --parameters ParameterKey=PrivateSubnet1CIDR,ParameterValue=REDACTED_KEYVALUE \
    --parameters ParameterKey=PrivateSubnet2CIDR,ParameterValue=REDACTED_KEYVALUE \
    --template-body file://REDACTED \
    --profile REDACTED
```