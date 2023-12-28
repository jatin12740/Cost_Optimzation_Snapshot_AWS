# Cost Optimization in AWS
##The Lambda function efficiently manages EBS snapshots within the AWS environment. By querying all EBS snapshots owned by the account, it dynamically compiles a list of active EC2 instances, encompassing both running and stopped instances. The function meticulously examines each snapshot, ensuring that the associated volume, if present, is not linked to any active instance.
##Upon identifying stale snapshots those no longer associated with any active instance the Lambda function takes proactive measures to optimize storage costs by promptly deleting them. This automated approach ensures the streamlined management of snapshots, aligning with cost-effective storage practices in AWS.
