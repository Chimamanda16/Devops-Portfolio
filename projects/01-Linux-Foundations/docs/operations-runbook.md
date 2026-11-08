# Northstar operations runbook

## Create a new group
`sudo groupadd [newgroupname]`

## Set ownership on folder
New owner: 
# Change owner only
`sudo chown [newowner]: foldername`

New group:
# Change group only
`sudo chown :[newGroup] foldername`

# Change owner and group
`sudo chown [newowner]:[newGroup] foldername`

## Set permissions on directory
`sudo chmod 2770 [directory_path]`

2 is for sgid
swap out 770 with numbers that represent the actual permissions you want to set

## Onboard a new employee
Create the new employee's account and add them to their corresponding groups
`sudo useradd -m -G [user's group] [newuser]`

### Note: use the `-G` flag and not `-g` in order to add the group as a supplementary group. The primary group should remain the user's private group

Set the new employee's password
`sudo passwd [newuser]`

## Offboard an employee
Delete emplyee and their files
`sudo userdel -r [username]`

Delete employee and retain their files
`sudo userdel [username]`


## Basic troubleshooting steps for access issues
+ Identify exact access issues
+ Find out what the correct access should be and compare with current behaviour
+ Find root cause of the access issues
+ Fix the issue

## Note: [] is used to indicate parameters that you should change. You are not to inlcude the square brackets when running the commands unless it is explictly specified to