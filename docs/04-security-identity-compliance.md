- IAM is a AWS service to management users access and permission;
- As well Organization SCP, IAM define the users permissions and actions conditions in AWS account;
- Root Account or Master Account is not a IAM user;
- IAM users are to employers accounts and integration service accounts;  
- It is possible to create polices to allow users access Organization through other organizations;
- It is good pratice to create one account only by Indentity purposes, from it, go to specifics accounts defined by policies (Switch Role);
- For operation purposes, dont use Root Account and Master Account, these accounts is most powerfull roles;
- It is suggested store Root Account and Master Account password with Dual-custody Authentication, break password and give to differents teams responsible;
- The account is create with numerical random ID number. The IAM service it is possible create an alias to URL organization account console, to delivery to employers IAM users;
- The IAM service it is possible create Group and Users. There is Policies for Groups and Users;
- Custom policies can be made;
- To easy the permissions downgrading, It is a goog pratice have attached `ReadOnlyAccess` and `FullAccess` Group or User police;
- Explicit in username if user is a service integration user, It is used `svc-*` prefix normally;  
- There is two options to AWS access type: Programatic Access (login with Token, for dev-tools, CLI, SDK); and AWS Management Console Access (for Employers); 
- It is possible set permission to User with following permission: Group, Copy permission from existing user, and Attach existing policies directly. The User can have permissions defined with one more type.
- User Tag assist in filters;
- Role is a mecanism to allow resources AWS to communicate with other AWS services;

## References

- AWS Well-Architected Tool
> - https://aws.amazon.com/well-architected-tool/

- AWS Well-Architected Doc
> - https://aws.amazon.com/architecture/well-architected/

- The 5 Pillars of the AWS Well-Architected Framework
> - https://aws.amazon.com/blogs/apn/the-5-pillars-of-the-aws-well-architected-framework/

