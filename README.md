# Infrastructure as Code

## Create Stack

### Serval parameters need to be passed in by command line


#### Create Networking Stack
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

#### Create Application Stack (Networking Included)
```
aws cloudformation create-stack \
    --stack-name csye6225demo \
    --parameters \
        ParameterKey=EnvironmentName,ParameterValue=REDACTED_KEYVALUE \
        ParameterKey=VpcCIDR,ParameterValue=REDACTED_KEYVALUE \
        ParameterKey=Region,ParameterValue=REDACTED_KEYVALUE \
        ParameterKey=SubnetCIDR,ParameterValue=REDACTED_KEYVALUE \
        ParameterKey=EC2InstanceType,ParameterValue=REDACTED_KEYVALUE \
        ParameterKey=EC2InstanceVolumeSize,ParameterValue=REDACTED_KEYVALUE \
        ParameterKey=DBInstanceType,ParameterValue=REDACTED_KEYVALUE \
        ParameterKey=DBInstanceVolumeSize,ParameterValue=REDACTED_KEYVALUE \
        ParameterKey=DBUsername,ParameterValue=REDACTED_KEYVALUE \
        ParameterKey=DBPassword,ParameterValue=REDACTED_KEYVALUE \
        ParameterKey=AMIID,ParameterValue=REDACTED_KEYVALUE \
    --template-body file://REDACTED \
    --capabilities CAPABILITY_NAMED_IAM \
    --profile REDACTED
```
