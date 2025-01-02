# aws-cli-commands

aws cloudformation list-stacks --stack-status-filter ROLLBACK_COMPLETE --query "StackSummaries[*].StackName" --output text | xargs -n 1 -I {} aws cloudformation delete-stack --stack-name {}
