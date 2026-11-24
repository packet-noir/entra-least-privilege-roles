## Exercise
Review six realistic tickets and identify the least privileged built-in role needed to resolve each one.

Compare your answers with Microsoft's: 
[Least privileged roles by task](https://learn.microsoft.com/en-us/entra/identity/role-based-access-control/delegate-by-task)

## Tickets
1. Reset the password for a salesperson who is locked out: **Password Administrator**
2. Create an account for a new hire starting Monday: **User Administrator**
3. Create a new security group for the Finance team: **Groups Administrator**
4. Give the systems admin the ability to create user accounts: **User Administrator**
5. Look at sign-in logs to investigate a suspicious login: **Reports Reader**
6. Reset the password for another administrator: **Helpdesk Administrator** (MSFT says: *User Administrator*)

## Corrections
Answering #6 was challenging since there are different types of administrators. I went with Helpdesk Administrator based on its description:

```
Helpdesk administrators can reset passwords ... of non-administrators or [users] assigned the following roles only:

    Directory Readers
    Guest Inviter
    >>Helpdesk Administrator<<
    Message Center Reader
    >>Password Administrator<<
    Reports Reader

```
#### Initial Reasoning
I chose not to assign the **User Administrator** role.

Granting permissions to create and manage user accounts and groups seemed excessive.
