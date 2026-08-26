**AWS Config**

- Helps with _auditing and recording compliance of your AWS resources_;
- Helps record configurations and changes over time;
- Possibility of storing the configuration data into S3 (analyzed by Athena);
- Questions that can be solved by AWS Config:
  - Is there unrestricated SSH access to my security groups?;
  - Do my buckets have any public access?
  - How has my ALB configuration changed over time?
- You can receive alerts (SNS notifications) for any changes;
- AWS Config is a pre-region service;
- Can be aggregated across regions and accounts;

---
