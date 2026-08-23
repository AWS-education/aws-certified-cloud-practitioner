**Why make a global application?**

- A global application is an application deployed in multiple geographies;
- On AWS: this could be _Regions_ and / or _Edge Locations_;
- _Decreased Latency_:
  - Latency is the time it takes for a network packet to reach a server;
  - It takes time for a packet from Asia to reach the US;
  - Deploy your applications closer to your users to decrease latency, better experience;
- _Disaster Recovery (DR):_
  - If an AWS region goes down (earthquake, storms, power shutdown, politics), ...;
  - You can fail-over to another region and have your application still working;
  - A DR plan is important to increase the availability of your application;
- _Attack protection:_ distributed global infrastructure is harder to attack;

---
