**Billing and Costing Tools**

- Estimating costs in the cloud:
  - Pricing Calculator;
- Tracking costs in the cloud:
  - Billing Dashboard;
  - Cost Allocation Tags;
  - Cost and Usage Reports;
  - Cost Explorer;
- Monitoring against costs plans:
  - Billing Alarms;
  - Budgets;

---

**AWS Pricing Calculator**

- Available at https://calculator.aws/;
- Estimate the cost for your solution architecture;

---

**Tracking Costs in the Cloud - Billing Dashboard, Cost Allocation Tags, Reports**

**Cost Allocation Tags**

- Use cost allocation tags to track your AWS costs on a detailed level;
- AWS generated tags:
  - Automatically applied to the resources you create;
  - Starts with Prefix **aws**: (e.g.: aws: `createdBy`);
- User-defined tags:
  - Defined by the user;
  - Starts with the prefix `user`;

**Cost and Usage Reports**

- Dive deeper into your AWS costs and usage;
- The AWS Cost & Usage Report contains _the most comprehensive set of AWS cost and usage data available_, including additional metadata about AWS services, pricing, and reservations (e.g., Amazon EC2 Reserved Instances (RIs));
- The AWS Cost & Usage Reports lists AWS usage for each service category used by an account and its IAM users in hourly or daily line items, as well as tags that you have activated for cost allocation purposes;
- Can be integrated with Athena, Redshift or QuickSight;

**Cost Explorer**

- Visualize, understand, and manage your AWS costs and usage over time;
- Create custom reports that analyze cost and usage data;
- Analyze your data at a high level: total costs and usage accross all accounts;
- Or Monthly, hourly, resource level granularity;
- Choose an optimal _Savings Plan_ (to lower prices on your bill);
- Forecast usage up to 12 months based on previous usage;

---

**Monitoring Costs in the Cloud - Billing Alarms & AWS Budgets**

**Billing Alarms in CloudWatch**

- Billing data metric is stored in CloudWatch us-east-1;
- Billing data are for overall worldwide AWS costs;
- It's for actual cost, not for projected costs;
- Intended a simple alarm (not as powerful as AWS Budgets);

**AWS Budgets**

- Create budget and send alarms when costs exceeds the budget;
- 4 types of budgets: Usage, Cost, Reservation, Savings Plans;
- For Reserved Instances (RI):
  - Track utilization;
  - Supports EC2, ElasticCache, RDS, Redshift;
- Up to 5 SNS notifications per budget;
- Can filter by: Service, Linked Account, Tag, Purchase Option, Instance Type, Region, Availability Zone, API Operation, etc, ...;
- Same options as AWS Cost Explorer!;

---
