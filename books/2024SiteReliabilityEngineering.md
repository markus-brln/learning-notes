SRE

### Chapter 1

- Dev and ops speaking different languages, different targets (deploy changes as soon as possible, no changes to keep
  things stable)
  - How to make this difference smaller at my company?
  - How to make developers take ownership of their operational problems like failing pods? Is it even feasible to have
    them on-call or sth? If stuff breaks devops will have to fix it anyway, maybe not familiar with the team's
    kubernetes setup and special hacks to make it work
- 100% availability shouldn't be the goal, consider error budget (product question), with that mindset outages are a
  natural part of progress, managed rather than feared. End users on a 99% reliable phone won't notice the difference
  between 99.9% and 99.99% uptime
- Monitoring: some monitoring output can create a ticket, not an alert. Rest is just logs
- Google has on-call playbooks

### Chapter 2+3

- Jealous of Google because they can make their own custom solutions for everything, like kubernetes is just an open
  source descendant of their internal specialized orchestration system
- Provide infra with different characteristics, e.g. High and low latency storage to suit their needs for error budgets,
  thereby reducing cost
- Tension between infra and dev teams about speed of development. Evaluated on reliability vs features, respectively ->
  discuss error budget together. Pushes possible until error budget is used, evaluate once per quarter using monitoring
  system

### Chapter 4

- Don't over-achieve beyond your SLOs, controlled outages/no lower latency under light load to prevent over-reliance on
  a service/system
  - Should really take nodes offline randomly
- Stricter SLO internally than externally to be able to respond quicker before externals will notice

### Chapter 5

- Eliminate toil
  - Manual and repetitive tasks are often toil. You do need human judgement to do it, but that may just mean that the
    underlying system is poorly designed (e.g. we have to do some magic with galera to make the whole thing work, we
    could have 2 dbs to switch in between or whatever other solution)
  - Solve e.g. by automating user provisioning
- Writing documentation is a way for me to reduce toil. Then devs don't have as many questions. Probably already
  saved me more hours than I spent documenting.

### Chapter 6

- Monitoring should have few noise (false alarms)
- When monitoring latency, also monitor error latency to get clues about why errors happen
- Measuring 99th percentile response time over a short time frame like a minute can be an early signal of saturation of
  a service
- Bucket latencies, make histograms, don't rely on the mean -> small part of requests that take long can be problematic
  and non-detectable with the mean
- Increase resolution of measurements and decrease cost by aggregating on the machines, and then collecting the data
  once a minute for example
- Make monitoring (alerting) decisions with long term goals in mind -> infrequent alerts today can become very frequent
  with code changes -> automate alert response?
- Escalate if you think your team can't clean up technical debt, and it's piling up
- A hit to availability may be worth it, turning off noisy alerts, thereby reducing distraction by them and fixing
  things long-term
