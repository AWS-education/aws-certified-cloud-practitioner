**ECS**

- ECS = Elastic Container Service;
- Launch Docker containers on AWS;
- _You must provision & maintain the infrastructure (the EC2 instances)_;
- AWS takes care of starting / stopping containers;
- Has integrations with the Application Load Balancer;

---

**Fargate**

- Launch Docker containers on AWS;
- _You do not provision the infrastructure (no EC2 instances to manage) - simpler!_;
- Serverless offering;
- AWS just runs containers for you based on the CPU / RAM you need;

---

**ECR**

- ECR = Elastic Container Registry;
- Private Docker Registry on AWS;
- This is where you store your Docker images so they can be run by ECS or Fargate;

---
