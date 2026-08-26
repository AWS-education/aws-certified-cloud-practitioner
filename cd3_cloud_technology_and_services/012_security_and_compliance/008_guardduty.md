**Amazon GuardDuty**

- Intelligent Threat discovery to protect your AWS Account;
- Uses Machine Learning algorithms, anomaly detection, 3rd party data;
- One click to enable (30 days trial), no need to install software;
- Input data includes:
  - CloudTrail Event Logs - unusual API calls, unathorized deployments:
    - CloudTrail Management Events;
    - CloudTrail S3 Data Events;
  - VPC Flow Logs - unusual internet traffic, unusual IP address;
  - DNS Logs - compromised EC2 instances sending encoded data within DNS queries;
  - Optional Features - ...;
- Can setup _EventBridge rules_ to be notified in case of findings;
- EventBridge rules can target AWS Lambda or SNS;
- Can protect against CryptoCurrency attacks (has a dedicated "finding" for it);

---
