# AWS LAMBDA FUNCTION - STALE EBS

### DESCRIPTION :
This Lambda function scans for all EBS snapshots owned by the account ('self') and gathers a list of active EC2 instances, including both running and stopped instances. For each snapshot, the function verifies if the corresponding volume, if it exists, is not linked to any active instance. If a redundant snapshot is detected, it is removed, optimizing storage expenses.
