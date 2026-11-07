# Northstar Incident report

## Incident Summary
Northstar developer, janedev has access to security file. THis is an access issue as she is not part of the security and compliance team

## Investigation steps
Tried to find out why janedev has access to the security team's files. It oculd either ne that she has mor access than she should or that the security team's folder has the incorrect groups assigned

## Root cause
janedev was incorrectly assigned to both the developers group and the security group

## Actions taken
janedev's group was correctly reassigned to prevent access to restricted files

## Verification
janedev no longer has access to the security team's folders

## Note
View the [evidence report](../evidence/) to see a more detailed report about this incident