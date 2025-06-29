# report-the-usage-of-aws-shellscript

##code for report the aws resources through script

   #!/bin/bash
########################
#This script will report aws resources  usage
set -x ##script in  debugging mode 
#author:vani
#aws s3
#aws lambda
#aws Ec2
#aws iam users
####################################
 echo "print s3 bucket"
aws s3 ls

echo "print ec2 instance"
aws ec2 describe-instances

echo "print lambda"
aws lambda list-functions

echo  "print iam"
aws Iam list-users


