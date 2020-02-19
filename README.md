# Infrastructure as Code

## Create Stack
```
aws cloudformation create-stack \
--stack-name REDACTED \
--parameters ParameterKey=REDACTED_KEYNAME,ParameterValue=REDACTED_KEYVALUE \
--template-body file://REDACTED \
--profile REDACTED
```