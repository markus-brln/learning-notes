# The Unicorn Project

Follow-up book of `The Phoenix Project`, now from the perspective of a lower-level manager/DevOps engineer.

### Chapter 1

- Devs need good dev environments that are easy to set up and dev onboarding, so they can actually be productive.

### Chapter 2

- Keep a work diary, including lessons on what to do and what not to do.

### Chapter 3

- Devs should be up and running within a day -> works really well at Belsimpel, need to appreciate things we take for
  granted -> good dev environment very important for all the new microservices.
- Test code very early on, so that it can be tested again for each change, so you only have to fix one thing at a time.

### Chapter 4

- Devs need to see their own changes in the test and production environments and get feedback from it, not just hand
  their feature to the next department.
- Projects should use a limited amount of technologies and be built by a small number of teams.

### Chapter 5

- Company shouldn't have a black market with favors between colleagues to fix supply and demand problems between teams.
- PRDs made sense decades ago, but now you can prototype features in the same time it takes to write the doc -> probably
  depends on how extensive the PRD is.

### Chapter 7

- Teams should work on one project that is relatively independent of others (loose coupling), otherwise communication
  and bureaucracy become too much.
- First ideal: locality and simplicity.

### Chapter 8

- The author is in love with functional programming.
- Devs should be able to write code, test it (manually), and push to production by themselves, quality assurance teams
  should be able to focus on higher-order tests.
- Also: access production logs
- Amazon "two-pizza teams" -> teams working independently that can be fed with 2 pizzas each.
- Sometimes it feels great to be at the center of everything, fixing things and picking up requests from people, but
  it's not sustainable.
- Microsoft: choice between working on a feature vs. dev productivity -> choose the latter.

### Chapter 9

- Same ticketing system for all dev teams with read access to everything.

### Chapter 10

- Devs should be able to merge changes to production themselves, since they know best what it does (also direct
  feedback, accountability).

### Chapter 11

- Committees like architecture should try to not block devs from coming up with new technology initiatives.
- If possible, teams create, test, and deploy their features by themselves.

### Chapter 12

- API strategy needed.
- Too many bash scripts for infra are bad.
- People with knowledge of where the product needs to go need to work closely together with the developers, otherwise
  it's way too much waiting for answering questions and getting feedback -> POs.

### Chapter 13

- Blameless post-mortems - absence of fear -> honesty -> prevention.
- Technologists should see once in a while what their work does at the front lines.

### Chapter 14

- Team names help create group identity and reinforce the importance of team goals over individual goals.
- Important to have vocabulary align across the company.
- Shouldn't forget the needs of the data science team in infra plans and when choosing technologies.
- They are making a central event bus -> basically it enables knowledge (data) sharing across the whole organization.

### Chapter 15

- Need to gracefully handle cases where 3rd party services are failing.

### Chapter 17

- Core vs. context, stopping/outsourcing the projects that don't contribute directly to the core business goals, can
  also re-assign context resources to core.
- Make sure to not work on context that should maybe be outsourced -> hosting GitLab? Probably depends on maintenance
  cost vs. cost of the service.

## Some AI generated summaries

### The Five Ideals:

- Locality and Simplicity: Emphasizing the importance of keeping systems simple and close to the work being done,
  reducing complexity to enhance efficiency and effectiveness.
- Focus, Flow, and Joy: Encouraging a state of focus and flow in work, aiming for joy in the process to improve
  productivity and satisfaction.
- Improvement of Daily Work: Stressing the continuous improvement of everyday tasks to gradually build a better overall
  system.
- Psychological Safety: Highlighting the necessity of creating an environment where people feel safe to take risks and
  innovate without fear of failure.
- Customer Focus: Focusing on the needs of the customer to guide decision-making and ensure alignment of efforts towards
  delivering value to the customer.

#### Examples to improve:

##### Locality and Simplicity

- Improve: Transition to a microservices architecture to allow teams to work independently, reducing coordination
  overhead.
- Improve: Simplify the system by breaking it down into smaller, loosely coupled modules, making it easier to manage and
  update.

##### Focus, Flow, and Joy

- Improve: Streamline workflows to minimize distractions and increase focus on core tasks.
- Improve: Implement agile methodologies to foster iterative development, enhancing team morale and job satisfaction.

##### Improvement of Daily Work

- Improve: Dedicate resources to regularly refactor code to reduce technical debt.
- Improve: Use automation tools to streamline repetitive tasks, freeing up time for more strategic work.

##### Psychological Safety

- Improve: Create a culture where mistakes are seen as learning opportunities, not failures.
- Improve: Encourage open communication and feedback loops to build trust within the team.

##### Customer Focus

- Improve: Conduct regular customer interviews to understand their needs and adjust product development accordingly.
- Improve: Prioritize features that directly address customer pain points to drive product differentiation.

### Context vs. Core

In "The Unicorn Project," core refers to activities that directly contribute to creating products or services that
customers are willing to pay for, establishing a competitive advantage. Context encompasses all other activities that
support the business but do not directly impact customer value or competitive edge, such as payroll systems or email
management. Shifting more towards core activities is encouraged to maximize investment in what truly matters to the
business and minimize expenditure on non-critical tasks. This approach aims to enhance the quality and competitiveness
of the core offerings while recognizing that some aspects of the business, though necessary, do not directly contribute
to customer satisfaction or competitive advantage.

To shift more towards core activities, consider the following strategies:

- Prioritize Feature Development: Focus on developing features that directly address customer needs and differentiate
  your product in the market.
- Outsource Non-Core Functions: Identify functions that are not central to your product or service offering and explore
  outsourcing options to free up resources for core activities.
- Automate Repetitive Tasks: Automate routine, non-core tasks such as reporting or data entry to reduce manual effort
  and allow team members to focus on core responsibilities.
- Review and Refine Processes: Regularly review processes to identify inefficiencies and redundancies, then streamline
  or eliminate non-core processes to allocate resources more effectively.
- Enhance Collaboration: Foster closer collaboration between departments to ensure that all activities align with the
  core mission and objectives, eliminating distractions and focusing on what truly drives success.
