# Principle of Least Privilege at Northwind

## Project Overview
This repository continues the Northwind Services identity management lab started in the [entra-directory-foundation](https://github.com/packet-noir/entra-directory-foundation) repository. It documents decisions and actions related to assigning administrative roles and determining who receives them.


## Business Scenario
IT staff at Northwind need certain permissions to perform their jobs. In this project I assess available built-in roles in Entra's free tier to assign the least privilege role against a given task. 

## Tools Used

Microsoft Entra ID (Free)
Microsoft Learn Docs
Github

## What I Built
Assigned least privilege roles to three IT staff members at Northwind. Created two break-glass accounts. Documented gaps in break-glass account state.

## Screenshots

### Role List

![List of roles](/screenshots/roles_list@2x.png)

### Assigned Role

![Role mapped to user](/screenshots/assigned-role@2x.png)

### Insufficient Permissions

![Missing the Create Users capability](/screenshots/permission_boundary_for_helpdeskadmin@2x.png)

### Role Assignment Audit Logs

![Role management logs](/screenshots/roleassignment_activity_logs@2x.png)

## Security Lessons Learned

The principle of least privilege is about precisely mapping an appropriate set of permissions to the right targets, without giving users more control and access than their role requires. 

## Future Improvements

Leverage additional features available in premium licenses like assigning roles to groups and privileged access management.
Cover gaps in break-glass account security like MFA setup and alerting.
