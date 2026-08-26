**Data at rest vs. Data in transit**

- _At rest_: data stored or archived on a device:
  - On a hard disk, on a RDS instance, in S3 Glacier Deep Archive, etc.
  - Encrypted at rest can be: Encrypted at rest on EFS, Encrypted at rest on S3;
- _In transit_: data being moved from one location to another;
  - Transfer from on-premises to AWS, EC2 to DynamoDB, etc;
  - _Means data transferred on the network_;

We want to ecrypt data in both states to protect it. To achieve this we can leverage **encryption keys** !

---

**AWS KMS (Key Management Service)**

- Anytime you hear "encryption" for an AWS service, it's most likely KMS;
- KMS = AWS manages the encryption keys for us;
- _Encryption Opt-in_:
  - EBS volumes: encrypt volumes;
  - S3 buckets: Server-side encryption of objects (SSE=S3 enabled by default, SSE-KMS opt in);
  - Redshift database: encryption of data;
  - RDS database: encryption of data;
  - EFS drives: encryption of data;
- _Encryption Automatically enabled_:
  - CloudTrail Logs;
  - S3 Glacier;
  - Storage Gateway;

---

**CLoudHSM**

- KMS => AWS manages the software for encryption;
- CloudHSM => AWS provisions encryption _hardware_;
- Dedicated Hardware (HSM = Hardware Security Module);
- You manage your own encryption keys entirely (not AWS);
- HSM device is tamper resistant, FIPS 140-2 Level 3 compliance;

---

**Types of KMS Keys**

- Customer Managed Key (Create, manage, and used by the customer, can enable and disable);
- AWS Managed Key (Created, managed, and used on the customer's behalf by AWS, ex: `aws/s3`);
- AWS Owned Key (Collection of CMKs that an AWS service owns and manages to use in multiple accounts);
- CloudHSM Keys (Keys generated from your own CloudHSM hardware service);

---
