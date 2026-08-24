**Amazon EventBridge (formly CloudWatch Events)**

- Schedule: Cron jobs (scheduled scripts):
  - Schedule Every hour -> Trigger script on Lambda function;
- Event Pattern: Event rules to react to a service doing something:
  - IAM Root User Sign in Event -> SNS Topic with Email Notification;
- Trigger Lambda functions, send SQS / SNS messages, ...;

---

**Events**

- Default Event Bus;
- Partner Event Bus;
- Custom Evenet Bus;

---
