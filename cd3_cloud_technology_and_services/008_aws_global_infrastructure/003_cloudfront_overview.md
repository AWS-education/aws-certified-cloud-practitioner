**AWS CloudFront**

- Content Delivery Network (CDN);
- Improves read performance, content is cached at the edge;
- Improves users experience;
- Hundres of Points of Presence globally (edge locations, caches);
- DDoS protection, integration with Shield, AWS Web Application Firewall;

---

**CloudFront - Origins**

- _S3_:
  - For distributing files and caching them at the edge;
  - For uploading files to S3 through CloudFront;
  - Secured using Original Access Control (OAC);
- _VPC Origin_:
  - For applications hosted in VPC private subnets;
  - Provate Application Load Balancer / Network Load Balancer / EC2 Instances;
- _Custom Origin (HTTP)_:
  - S3 website (must first enable the bucket at a static S3 website);
  - Any public HTTP backend you want (example: Public ALB);

---
