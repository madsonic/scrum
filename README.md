# Scrum
Framework for managing complex adaptive problems.

# Principles of scrum
1. Bring highest value to customer at delivery date
2. Transparency

# Roles of a Scrum Team
1. Product Owner (PO)
2. Scrum Master (SM)
3. Development Team (Devs)

The size of the scrum team ranges from 3-9 people

## Product Owner
The product owner is responsible for maximising the value of the product. He
spends time understanding the needs of the users/stakeholders and has a clear 
vision of the product even though at time he might need to consult the 
users/stakeholders. He owns the product backlog and ultimately the scope,
schedule, cost and quality of the project.

## Scrum Master
The scrum master ensures that everyone is clear about scrum and that its rules
they are followed. He facilitates the Sprint, fosters transparency and remove
any impediments that the slows down the Devs and protects that from any
distractions that stops them from reaching the sprint goals.

## Development Team
The development team consists of the people that actually do the work set out in
the sprints. They are self-organising meaning they manage, organise and allocate
the work themselves. They are also cross-functional. The team collectively is
able to design, program, test (i.e. have multiple domain knowledge). It is
possible that they are cross-trained (someone who can program and test, design,
program and test, etc).

It is recommended though not necessary that each role is played by a different
individual in the team. However according empirical observations this is not the
case commonly due to differences in organisational structure, budget constraints 
or other reasons. Therefore it is not uncommonn to see the following:
1. PO in multiple scrum teams
2. SM in multiple scrum teams
3. SM & Dev roles done by same person (usually someone who always plays as Dev)
4. PO & SM (not recommended)

While 1, 2 and 3 are still ok, 4 is discouraged because there can be
tendencies to micromanage, pressure and scrutinise dev actions which can result
in lower productivity, less transparency and eventually lower quality product.
The tendency arises because of the SM works very closely together with the Devs.
However there can be exceptions depending on the person.

# Practices of Scrum
The most distinctive practice of scrum is the sprint cycle. It consists of 3
phases - plan, sprint and review & retrospective. It is also known as plan,
product and inspect & adapt.

In scrum, we focus on things left rather than things done. You will see that
estimates, time, charts, etc deal with what is left rather than what has been
used. In short, what remains is more important.
## Sprint Cycle
The sprint cycle is timeboxed at 2 weeks long (no hard and fast rule but
recommended to be shorter than 4 weeks long). During the cycle the Devs tries to
achieve the sprint goal

### Sprint planning
Each cycle begins with **sprint planning** for Devs to decide on the sprint
goal. Planning is timeboxed at 2h x weeks in a sprint. Planning can involve the
entire scrum team. The Dev will translate the PBIs into a sprint backlog which
is a list of actionable tasks. The Devs will also decide on the 'Definition of
done' (DoD) in the first sprint planning. Although DoD can be changed later on,
it is best to decide on something reasonable and stable early on to minimise
confusion.

The plan should typically include some buffer time to deal with unplanned events
like hotfixes, security vulerability, investigations, etc.

#### Capacity based sprint planning
Capacity is calculated in time units e.g. hours or quarter days. An example
planning looks like this.

> Weeks in sprint = 2
> Total working hours in a sprint = 2 weeks * 5 days * 9 hours = 90
> Size of Dev team = 5
> Total manhour in a sprint = 90 * 5 = 450

There can be deduction in hours due to holidays, planned leave or training, etc.

More fine-grained role based hours can be helpful. Instead of total manhour, we
calculate total manhour for a particular role

> Number of programmer = 3 -> total programming hours = 90 * 3 = 270
> number of designer   = 1 -> 90
> number of tester     = 1 -> 90

In the case where there is a cross trained individual i.e. programmer and
tester, the same calculations can be used but the time spent on each type of
task must be decided beforehand i.e. John will spend half his time programming
and the other half testing.

### Sprint
The bulk of the time will be spent trying to mark tasks in the sprint backlog as
done. 

#### Daily Standup
During the sprint, the Devs & the scrum master hold a daily standup to give a
brief update to themselves of the following:
1. What I have done yesterday
2. What I am going to do today
3. Am I facing any impediments/issues/blockers

Daily standup is timeboxed at 15mins regardless of the size. It is important that
the daily standup to be an 'update' rather than a discussion. Everyone states
the 3 points and move on to the next member. Any discussions should be done
after. Issues can be tracked on a impediments backlog if it requires the help of
the SM.

After the daily standup, the sprint backlog and sprint burndown chart will be
updated.

The sprint backlog looks something like this:

PBI | Not Done | Doing | Done
--- | -------- | ----  | ---
#1  | taskA <3h> | taskB <1h> \<John\> | taskC <2h> \<Tom\>
... | ... | ... | ...


The tasks can only be marked as done when it fulfills 'definition of done' (DoD).

#### Definition of Done
The definitions stated should be easily verifiable. It is either passes or not,
no gray area.

Sample of check list for a task to be considered done.
- PO acceptance
- code checked in
- code reviewed
- unit, integration, performance tests pass
- passes other non-functional requirements
- no P0, P1 defects
- updated documentation

### Sprint Review & Retrospective
The focus of the review is the product. During the review, anyone interested in
the product is invited for hands-on with the product. They can be end-users,
stakeholders or members from other scrum team. The team will share the 
current state of the product and also discusses with everyone on how to maximise
delivering value. e.g. changes to the product backlog.

On the other hand, the focus of the retrospective is the sprint process. This
typically only involves the scrum team. They inspect the processes internally
and review how the sprint went so that they might try something new in the next
sprint. 

One way to conduct restrospective is to use the 'Start, Stop, Continue'
technique to find out what practices should continue, start and stop in the next
sprint.

If any issues is voiced out during the retrospective, it can be kept in a
impediments backlog for the SM to take action.

At the end of each sprint, the PO also updates his release burndown chart
(remaining size of product backlog against remaining sprints)

## Product backlog
Priority list of product backlog items (PBI) sorted in descending order by return
on investment (ROI). ROI is however you define it to be but commonly as
Value / Effort and value can be one of business value, engineering value or other
perceived value.
Because of how the backlog is sorted, the items with the highest ROI are tackled
first, long before the release date and the highest value are 'locked in' to
the product early on. 

This is solely owned by the PO; he decides on the content of the PBI as
well as their order. He can consult anyone including by not limited to
stakeholders, users, scrum master, development team and legal team

Although the order of PBI is decided before the start of the project, its order
can be changed throughout the project. For example, any time during the 
project, due to changing market needs, another item might have higher ROI
and the PO moves that item up. Or maybe there are dependencies, or for
efficiency reasons that some items are done together.

It is also wise to include some scope buffer which are typically items at the
bottom in case better ideas come along or estimates at the start were too
optimistic. In those cases, the least value items (at the bottom) are typically
dropped for the current release.

### PBI
The PBI typically includes a feature, size and value estimation

#### User stories
The feature part of PBI can be written as user stories which has 3 parts: **card**, **conversation**
and **confirmation**. The card is a high level use case written in this format
> As a user xxx
> I want to yyy
> so that zzz

The card will not have all the nitty gritty details needed for implementation so
that the PO and Devs **converse** to get **confirmations** from the PO.

The stories should typically be refined until it is small enough to be done in a
few days. Refinement is usually done a sprint before when the items are about
to be tackled. User stories can be sliced into smaller chunks by feature steps
or by business value. Feature steps are logical steps from technical point of
view. Business value gauges the ROI of the feature and groups them together.

#### Size Estimations - Planning Poker
This is done by the Devs to gauge the size of the PBI. Size = effort +
complexity + uncertainty.
A maximum of 3 rounds of scoring is done for each item. The scores used come from the
Fibonacci sequence. 0, 1, 2, 3, ..., 20 and includes infinity and '?'.
Infinity indicates the item is too large to estimate and needs to be broken down
further while '?' indicates that you have no clue. 

Each Dev member picks a score and reveals it **simultaneously**. 
Every member explains why they chose the score, starting with the highest, 
lowest and everyone else. It is important that no discussion happen, similar to
the daily standup; you state you opinion and continue with the next member.
When there is a consensus or by the end of round 3, the score is written on the
PBI. If a round 3 take place, the majority score is used or if there is a split,
the score in between if there is one or the higher score is written down. 

# Tools, techniques and Recommendations
## Practices improve flow

## Seating arrangement recommendation
Scrum team should be in the same room. In particular it has been observed that 
tester and programming seated side by side is very helpful, along with designer
and artitect very close by. But this all depends on the team composition and
how well it works out. Maybe it is better that the PO seats slightly further away
or not. It all depends on trial and error.

## Estimation techniques
Big complex items use relative estimate
- PBI. scoring system

Small item use absolute estimate
- sprint backlog items (tasks). hours, days, etc

### Fibonacci numbers
The nature of the sequence ensure that large items results in larger than normal
numbers. Large items has unforseeable complexities and uncertainties

## Release Date Estimation
## Velocity Estimation

## Sprint zero & Pre-release sprint
Sprint zero - kick off the project, research, infra setup, other
necessary tools setup, conventions agreement

Pre-release sprints - version tagging, release logs, actual release dates, ads,
marketing, announcements, invitations, development halts

# Glossary
Product backlog: descending list of items sorted by ROI.
Product backlog items: includes features, size estimates, and ROI
Sprint backlog: list of tasks need to be done to complete PBI
Sprint goals: number of PBIs to complete by end of a sprint
Timebox: Upper limits for actions
Definition of done: checklist to easily verify if task is done.
Daily standup: daily meeting to update scrum team on, done, doing and blockers
