**AWS Organizations**

- Global service;
- Allows to manage _multiple AWS accounts_;
- The main account is the master account;
- Cost Benefits:
  - _Consolidated Billing_ accross all accounts - single payment method;
  - Pricing benefits from _aggregated usage_ (volume discount for EC2, S3);
  - _Pooling of Reserved EC2 instances_ for optimal savings;
- API is available to _automate AWS account creation_;
- _Restrict account privileges using Service Control Policies (SCP)_;

---

**Multi Account Strategies**

- Create accounts per _department_, per _cost center_, per _dev_ / _test_ / _prod_, based on _regulatory restrictions_ (using SCP), for _better resource isolation_ (e.g.: VPC), to have _separate per-account service limits_, isolated account for _logging_;
- Multi Account vs One Account Multi VPC;
- Use tagging standards for billing purposes;
- Enable CloudTrail on all accounts, send logs to central S3 account;
- Send CloudWatch Logs to central logging account;

---

**Service Control Policies**

- Whitelist or blacklist IAM actions;
- Applied to _OU_ or _Account_ level;
- Does not apply to the Master Account;
- SCP is applied to all the _Users and Roles_ of the Account, including Root;
- The SCP does not affect service-linked roles:
  - Service-linked roles enable other AWS services to integrate with AWS Organizations and can't be restricted by SCPs;
- SCP must have an explicit Allow (does not allow anything by default);
- Use cases:
  - Resctrict access to certain services (for example: can't use EMR);
  - Enforce PCI compliance by explicitly disabling services;

---
