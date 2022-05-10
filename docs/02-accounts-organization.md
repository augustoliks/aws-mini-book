This section is about:

- Accounts Foundation;
- AWS Accounts;
- AWS Organization;
- SCP - Security Control Policy;
- Support Center Plans.

## Foundations

These important point about Accounts Foundation:

- Important on init Cloud Project;
- One account is not better way to utilize AWS Account;
- Does not exist Wrong, the wrong is not has strategy;
- AWS Account is cost less.

![02-account-diagram.drawio.png](img/02-account-diagram.drawio.png)

Hierarchical account strategy to better __Organization__ and __Security__.  This account strategy, the sub accounts is to organizate domain sections, centralize billing and restrict resource create permission based sub-account.

- __Master Account__: Composed by only one AWS Account. In this account, only _Root Account_ it used. This account is the first account created and is is to create or associate other sub-accounts. This account function is to unify sub-accounts billing only, no new __Resources__ should be created.

> :memo: _Root Account_ is the user who owns an AWS Account.

- __Oraganisation Unit - OU__: Visually organize AWS Accounts and service security rules. Normally, it was created to Domain Departaments.

> :memo: To indetify Domain Departaments, a one way is understood characteristic about the resources presents it. If Type, Lifecycle and, Permissions are differents, maybe it's a Department. 

- __Accounts__: Account when will be create resources and deployments. Each account has identity that associate resources created in it. The users should be created in this account.

- __Resources__: AWS services and resources, for example: EC2, S3, EKS, EFS etc.

Dont be confused Master Account with Root Account. Master Account is the first account created on AWS and Root Account is the user who owns an AWS Account.

__AWS Organization__ is important to create __Consolidated Billing__ feature. This feature is to centralize billing of the sub-accounts.

There are two ways to create sub-account. In `AWS Organization`, you can be create newer AWS account, or invite AWS existing account. Both ways are made given email. To accepted invite from AWS existing account, in console of the Existing Account, it should be access `AWS Organization` menu, and click accept invite option, the accept is not be done by email.

The create resource restriction can be _SCP - Security Control Policies_ that provides options to restrict resources creation to OU or Accounts.

## Account Security Pratices

- Active MFA for all account, specially Root Account.

- For create new accounts, it is necessary one unique email. The best pratice is create email group for the team and not used person emails.

- Add __Alternate Contacts__ in Root Account. It is important to receive security contacts from AWS Support.

## Accounts Support Center Plans

There is differents _AWS Support Plans_ levels: 

- __Basic__ (free): Recommended if you are experimenting or testing in AWS;
- __Developer__: Minimum recommended tier if you have production workloads in AWS;
- __Business__ Recommended if you have production and/or business critical workloads in AWS;
- __Enterprise__: Recommended if you have business and/or mission critical workloads in AWS.

## References

- AWS Account
> - [https://aws.amazon.com/account/](https://aws.amazon.com/account/)

- AWS Organizations
> - [https://aws.amazon.com/organizations/](https://aws.amazon.com/organizations/)

- AWS Support Center Plans
> - [https://aws.amazon.com/pt/premiumsupport/plans/](https://aws.amazon.com/pt/premiumsupport/plans/)

- AWS Landing Zone
> - [https://aws.amazon.com/solutions/aws-landing-zone/](https://aws.amazon.com/solutions/aws-landing-zone/)

- AWS Billing
> - [https://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/useconsolidatedbilling-procedure.html](https://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/useconsolidatedbilling-procedure.html)

- AWS SCP - Service Control Policies
> - Reference: [https://docs.aws.amazon.com/organizations/latest/userguide/orgs_manage_policies_scp.html](https://docs.aws.amazon.com/organizations/latest/userguide/orgs_manage_policies_scp.html)
> - Example: [https://docs.aws.amazon.com/organizations/latest/userguide/orgs_manage_policies_example-scps.html](https://docs.aws.amazon.com/organizations/latest/userguide/orgs_manage_policies_example-scps.html)
