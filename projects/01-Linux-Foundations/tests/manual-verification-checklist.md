# Manual Verification Checklist – Linux Foundations

Use this checklist to confirm that the Northstar Systems access control environment was implemented correctly.

## Identity & Groups
- [x] All required groups were created (`platform-eng`, `developers`, `security`, `operations`)
- [x] Representative users were created for each department
- [x] Users are members of the correct primary and supplementary groups
- [x] User accounts can be inspected with `id` and `groups`

## Filesystem Structure
- [x] `/srv/northstar` directory and all department folders were created
- [x] Sample files were created inside the department folders

## Ownership & Permissions
- [x] Each department folder has the correct group ownership
- [x] Permissions follow least privilege (others have no access where required)
- [x] Setgid bit is applied where needed so new files inherit the correct group
- [x] Shared folder allows read access but not write access for its group

## Access Verification
- [x] Authorized users can enter and use their department folders
- [x] Unauthorized users are denied access to restricted folders (especially `security`)
- [x] Shared folder access works as defined in the access policy

## Incident Investigation
- [x] A permission or ownership problem was deliberately introduced
- [x] Evidence was gathered before making changes
- [ ] Root cause was correctly identified
- [x] The smallest appropriate fix was applied
- [x] Access was re-tested after the fix (both allowed and denied cases)

## Documentation
- [x] Architecture, access policy, runbook, and incident report are completed
- [x] Evidence (screenshots or terminal output) has been added to the `evidence/` folder