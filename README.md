# Infrastructure as Code

## Create Stack

#### Serval parameters need to be passed in by command line

```
aws cloudformation create-stack \
    --stack-name REDACTED \
    --parameters \
        ParameterKey=EnvironmentName,ParameterValue=REDACTED_KEYVALUE \
        ParameterKey=VpcCIDR,ParameterValue=REDACTED_KEYVALUE \
        ParameterKey=Region,ParameterValue=REDACTED_KEYVALUE \
        ParameterKey=PublicSubnet1CIDR,ParameterValue=REDACTED_KEYVALUE \
        ParameterKey=PublicSubnet2CIDR,ParameterValue=REDACTED_KEYVALUE \
        ParameterKey=PublicSubnet3CIDR,ParameterValue=REDACTED_KEYVALUE \
    --template-body file://REDACTED \
    --profile REDACTED
```
