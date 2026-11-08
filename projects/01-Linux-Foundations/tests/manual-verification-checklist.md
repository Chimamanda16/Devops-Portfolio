# Manual Verification Checklist – Linux Foundations

Use this checklist to confirm that the Northstar Systems access control environment was implemented correctly.

## Identity & Groups
- [ ] All required groups were created (`platform-eng`, `developers`, `security`, `operations`)
- [ ] Representative users were created for each department
- [ ] Users are members of the correct primary and supplementary groups
- [ ] User accounts can be inspected with `id` and `groups`

## Filesystem Structure
- [ ] `/srv/northstar` directory and all department folders were created
- [ ] Sample files were created inside the department folders

## Ownership & Permissions
- [ ] Each department folder has the correct group ownership
- [ ] Permissions follow least privilege (others have no access where required)
- [ ] Setgid bit is applied where needed so new files inherit the correct group
- [ ] Shared folder allows read access but not write access for its group

## Access Verification
- [ ] Authorized users can enter and use their department folders
- [ ] Unauthorized users are denied access to restricted folders (especially `security`)
- [ ] Shared folder access works as defined in the access policy

## Incident Investigation
- [ ] A permission or ownership problem was deliberately introduced
- [ ] Evidence was gathered before making changes
- [ ] Root cause was correctly identified
- [ ] The smallest appropriate fix was applied
- [ ] Access was re-tested after the fix (both allowed and denied cases)

## Documentation
- [ ] Architecture, access policy, runbook, and incident report are completed
- [ ] Evidence (screenshots or terminal output) has been added to the `evidence/` folder