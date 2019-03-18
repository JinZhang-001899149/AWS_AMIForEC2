# AWS AMI for CSYE 6225

## Team Information

| Name | NEU ID | Email Address |
| --- | --- | --- |
|Jin Zhang|001899149|zhang.jin2@husky.neu.edu |
|Yanjuan Li|001497203|li.yanj@husky.neu.edu |
|Jingyi Cui|001493484|cui.jingy@husky.neu.edu |
|Xinxin Huang|001898856|huang.xinx@husky.neu.edu|

## Validate Template

```
packer validate ubuntu-ami.json
```

## Build AMI

```
packer build\
    -var 'aws_access_key=REDACTED' \
    -var 'aws_secret_key=REDACTED' \
    -var 'aws_region=us-east-1' \
    -var 'subnet_id=REDACTED' \
    ubuntu-ami.json
```
