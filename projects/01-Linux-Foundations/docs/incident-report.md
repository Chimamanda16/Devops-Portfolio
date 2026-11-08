# Northstar Incident report

## Incident Summary
Northstar developer, janedev has access to security file. This is an access issue as she is not part of the security and compliance team

## Expected state
janedev is not part of the security team and should not have access to security and compliance files and folders

## Investigation steps
I tried to find out why janedev has access to the security team's files. It could either be that she has more access than she should or that the security team's folder has the incorrect groups assigned

## Observed state
janedev currently has access to files and folders belonging to the security and compliance team

## Root cause
janedev was incorrectly assigned to both the developers group and the security group

## Actions taken
janedev's group was correctly reassigned to prevent access to restricted files

## Verification
janedev no longer has access to the security team's folders

## Prevention
Include a group inspection procedure during onboarding

## Note
View the [evidence report](../evidence/) to see a more detailed report about this incident