**S3 Storage Classes**

- Amazon S3 Standard - General Purpose;
- Amazon S3 Standard-Infrequent Access (IA);
- Amazon S3 One Zone-Infrequent Access;
- Amazon S3 Glacier Instant Retrieval;
- Amazon S3 Glacier Flexible Retrieval;
- Amazon S3 Glacier Deep Archive;
- Amazon S3 Intelligent Tiering;

! We can move between classes manually or using S3 Lifecycle configurations;

---

**S3 Standard - General Purpose**

- 99.99 % Availability;
- Used for frequently accessed data;
- Low latency and high throughput;
- Sustain 2 concurrent facility failures;
- Use cases: Big Data analytics, mobile & gaming applications;

---

**S3 Storage Classes - Infrequent Access**

- For data that is less frequently accessed, but requires rapid access when needed;
- Lower cost than S3 standard;

_S3 Standard-Infrequent Access_ (S3 Standard-IA)

- 99.9 % Availability;
- Use cases: Disaster Recovery, backups;

_S3 One Zone-Infrequent Access_ (S3 One Zone-IA)

- High durability (99.999999999 %) in a single AZ; data lost when AZ is destroyed;
- 99.5 % Availability;
- Use cases: storing secondary backup copies of on-premise data, or data you can recreate

---

**S3 Glacier Storage Classes**

- Low-cost object storage meant for archiving / backup;
- Pricing: price for storage + object retrieval cost

_S3 Glacier Instant Retrieval_

- Millisecond retrieval, great for data accesed once a quarter;
- Miminum storage duration of 90 days;

_S3 Glacier Flexible Retrieval_

- Expedited (1 to 5 minutes), Standard (3 to 5 hours), Bulk (5 to 12 hours) - free;
- Miminum storage duration of 90 days;

_S3 Glacier Deep Archive_

- Standard (12 hours), Bulk (48 hours);
- Miminum storage duration of 180 days;

---

**S3 Intelligent Tiering**

- Small monthly monitoring and auto-tiering fee;
- Moves objects automatically between Access Tiers based on usage;
- There are no retrieval charges in S3 Intelligent-Tiering;

_Tiering_

- Frequent Access tier (automatic): default tier;
- Infrequent Access tier (automatic): objects not accessed for 30 days;
- Archive Instant Access tier (automatic): objects not accessed for 90 days;
- Archive Access tier (optional): configurable from 90 days to 700+ days;
- Deep Archive Access tier (optional): configurable from 180 days to 700+ days;

---
