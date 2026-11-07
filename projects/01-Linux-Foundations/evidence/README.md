# Screenshots explanations for evidence documentation

## Fixed incorrect group assignment
**Problem**: johndev is a developer who no longer has access to development files. 
**Cause**: This was because the development folder was incorrectly assigned to the engineering group
**Fix**: Correctly assign the developers group to the development folder and remove the engineering group from the development folder

+ working-state-01.png - johndev who is a developer has proper access to the development folders and files
+ change-permissions-02.png - change the group of the development folder from the developers group to the engr group
+ broken-state-03.png - johndev no longer has access to the development folders and files
+ fixed-state-04.png - Correctly update the development folder's group to the developers group. johndev can now access the development folders and files

## Fixed leaast priviledge issues
**Problem**: janedev is a developer who incorrectly has access to the security and compliance files and folders. 
**Cause**: Janedev was incorrectly assigned to both the developers group and the security group
**Fix**: The user's group was correctly reassigned to prevent access to restricted files

+ janedev-least-priviledge-01.png - janedev can only access the development folder and not the securtiy-&-compliance-folder
+ janedev-incorrect-access-02.png - janedev is incorrectly part fo the security group and can now access security and compliance files
+ janedev-least-priviledge-fixed-03.png - reassigned janedev correctly to only development group, preventing access to restricted files

## Note
All referenced screenshots can be found in the [screenshots folder](screenshots/)