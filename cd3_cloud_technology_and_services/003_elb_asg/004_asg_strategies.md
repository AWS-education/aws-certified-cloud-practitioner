**Auto Scaling Groups (ASG) Strategies**

- _Manual Scaling_: Update the size of an ASG manually;
- _Dynamic Scaling_: Respond to changing demand:
  - _Simple / Step Scaling_:
    - If CPU > 70 %, then add 2 units;
    - If CPU < 30 %, then remove 1 unit;
  - _Target Tracking Scaling_:
    - I want the average ASG CPU to stay at around 40 %;
  - _Scheduled Scaling_:
    - Increase the min. capacity to 10 at 5 pm on Fridays;
- _Predictive Scaling_: Uses Machine Learning to predict future traffic ahead of time;

---
