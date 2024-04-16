### Goals

- Ship a milestone (working product)
- On budget, on time
- Figure out staffing of project
- Identify 1st release
    - Prioritize what’s important
- Identify additional releases
    - Only at a high level

### 4 Principles of Agile Planning

- Iterative product delivery by establishing milestones
- Be realistic
- Be quantitative (measure)
- Make measures visible

### Iteration (Sprint)

- A working piece of code to deliver to the customer
- We put stories into iterations, sort priorities first by H, M, L
- Should be 1-2 weeks
- Don’t split a story over multiple iterations
- Addresses the following risk: misunderstandings from customer, estimates are too optimistic, we re-plan if these things arise

### Milestone

- Working product that ships to the user
- Milestone 1.0
    - Baseline, Minimal Subset, Minimal Viable Product
    - We identify this from the customer but it’s also partly technical (need login to save account info)
    - Get over nice to haves
- Milestone 2.0
- Milestone N (Final Product)
- Addresses the risks:
    - Customer misunderstood user needs
    - Running out of money
    - Problems with working in the “real world”
- This is when developers get paid

### Correcting for Developer Optimism

- Two key adjustments
    - Count 20 days to a month
    - Velocity to account for work day efficiencies
        - Ex Calculation: 2 developers 10 days of work done in 20 days. Velocity = hours of work done/ work hours passed = 10 / 2*20 = 0.25 = 25%
    - Estimate Time to Complete Story = Hours of Work / Velocity
    - Estimated work that will get done = # of team members X working hours in an iteration * velocity
- Velocity only accounts for interruptions
- Initially guess then measure using previous iterations

### Translating User Stories into Tasks

- Customer oriented feature → code oriented functionality
- Need to update the user story estimate after breaking down into task estimates
- Task estimates based on who is likely to do the task
- It’s ok to have extra tasks and delete them
- Make sure we have story tests, please yourselves with story tests.
- Regression testing: going back to earlier and make sure everything still works
- Automated testing

### Big Board

- Track user stories, tasks in the user stories, tasks in progress, completed tasks, completed stories, bumped user stories to next iteration
- Where we find unplanned tasks
- Don’t spread tasks too thin

### Burn Down Chart

- Work left in hours vs Work time left in iteration
- If we’re plotting below line we’re ahead of schedule
- If we’re above line we’re behind schedule
- With every task we plot a new point
- Hours left is the number of ppl hours left so ppl x days