# The Phoenix Project 2024

### Chapter 1+2

- People need to be able to freely tell the boss bad news.
- In order to solve an issue, you need a timeline of events.

### Chapter 3

- Don't push a big update the afternoon before going on vacation. Maybe the day before.
- Conflict of interests between security team and DevOps (everything secure vs setting up new stuff).
- There need to be processes in place that allow people to actually get stuff done and coordinate with others to safely
  release changes (e.g., local dev setup, release flow).
    - All changes need to be documented in MRs and tickets, so you can trace back when something goes wrong.

### Chapter 5

- Meetings only for identifying next steps.
- Constant tension: security vs finishing projects.
- Very bad to have one person knowing everything, being needed for all complex projects.
- Management needs to know demand, priorities, status of work in process, and resource availability.
- When increasing the priority of one thing, the other thing being replaced shouldn't be forgotten as it also has a
  deadline.

### Chapter 6

- Better to analyze the whole situation than to only put out fires.
- Monitoring policies are important.
- During meetings, say things like "let's put this aside for now" in order to stay on topic.
- Need to find a way to get project work done and not get small requests all the time.
- "Marking requests as urgent is the only way they get picked up" - very bad situation.

### Chapter 7

- Work in progress needs to be kept under control; things need to get shipped.
- Theory of constraints: improvements anywhere outside the bottleneck are an illusion.
- Predictability of what work needs to be done is important in an organization.

### Chapter 8

- High-risk changes should be authorized by higher-ups.
- Ask other stakeholders, e.g. business, when they want us to do a high-risk change.
- Changes that have been done before on a regular basis can be approved automatically.
- Medium risk should be managed by lower-level managers, them making sure stakeholders are okay with the changes.

### Chapter 9

- Important: if something doesn't work, try to find the root cause instead of applying random fixes like restarts. That
  makes finding the root cause harder. Also, communicate and get approval for possible fixes.
- Reduce other changes made if a big one is scheduled.
- Four kinds of IT operations work: business projects (new features), internal IT operations projects (making things
  more efficient internally), changes (changes to existing systems, maintenance), unplanned work (see Chapter 15) ->
  avoid unplanned as much as possible, for that we need to focus more on 2 and 3.

### Chapter 10

- As DevOps engineer, really stop people from contacting you directly -> "Processes protect people."
- Also be aware yourself if you're distracting people from important projects.
- Documentation when you fix things -> how can incident reports be used as a knowledge base?
- People shouldn't hoard knowledge -> documentation.
- Weird but interesting solution, maybe for bigger organizations: a pool of people having access to very knowledgeable
  people. Those people with knowledge just advise and let the ones in the pool execute and document.

### Chapter 11

- If there's too much for the DevOps team, stop accepting it.
- If there is a bottleneck, it helps to know which things really need it and which things have workarounds.

### Chapter 12

- Versioning is important to keep track of what version is working and what isn't.
- Bad: database scripts that are expected to take long and can't be stopped without messing up the data -> changes in
  one transaction.

### Chapter 14

- Vicious cycle: more features needed in a product, forced to take shortcuts, worse deployments, more maintenance and
  bugs, more features (functional requirements) with technical debt (lacking technical requirements).
- Code done date != everything tested and deployed date -> needs to be communicated.
- Important that DevOps and devs have a good relationship.

### Chapter 15

- The problem with prevention is that you usually don't know about the disasters you averted.
- Bottlenecks: 1. Be sure that it's your bottleneck. 2. Keep it utilized for highest priority tasks at all times + it
  shouldn't have to wait on anything. 3. Find ways around the bottleneck to throttle input to it.

### Chapter 18

- Trust is necessary to prevent micromanaging (leadership skipping levels of delegation).

### Chapter 19

- Risk of operations work not factored into time estimations, only development -> still cleaning up shortcuts taken in
  Handyhelden like 2 months after -> not available for new projects, only by neglecting the unfinished one -> maybe
  we're the bottleneck right now?
- What's the mechanism of accepting work? -> if there is none, then we always pick up the latest high priority project
  and generate a lot of technical debt. Technical debt has compound interest in the form of unplanned work leaving no
  time for planning (vicious cycle), so make sure to pay it off in the short term.
- If you're the bottleneck, make sure our time is not "wasted" with other things  than the most important ones.
- Solution to improve due-date performance: stop new work from coming DevOps' way for some time, let them reduce the
  work in progress.

### Chapter 20

- First projects after project freeze can be the ones that don't require the bottleneck anymore. For that, you need to
  know what resources are required.
- "Improving daily work is more important than doing daily work."
- Prioritize work that increases throughput.

### Chapter 22

- Minimizing WIP (having few open tickets that are blocked) -> concepts like these should be communicated from that
  holistic perspective, so we understand why we should do it. E.g., How does workflow change X help the company?
- Again, it's important to work on projects that alleviate work from the bottleneck, it's an investment.

### Chapter 23

- Everyone in the system needs a bit of idle time because wait time = %busy / %idle, otherwise WIP gets stuck -> need to
  make time for processing WIP -> be able to pick up MRs and requests faster.

### Chapter 26

- Big role of development is that other teams in the company can do their work, e.g., making sales observable.
- Time to market is important, otherwise money for R&D could have just been invested somewhere else.

### Chapter 27

- In order to avoid threatening business goals, it needs internal compliance rules, e.g., keeping software up-to-date,
  which reduces the amount of firefighting and outages -> take internal compliance seriously.
