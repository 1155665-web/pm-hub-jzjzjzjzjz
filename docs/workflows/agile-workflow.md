# Agile Workflow Guide

## What is Agile?

Agile is an iterative approach to software development that emphasizes flexibility, collaboration, and customer feedback. Rather than planning everything upfront, Agile teams work in short cycles (sprints) to deliver value incrementally.

## Core Agile Principles

1. **Individuals and interactions** over processes and tools
2. **Working software** over comprehensive documentation
3. **Customer collaboration** over contract negotiation
4. **Responding to change** over following a plan

## Agile Frameworks

### Scrum (Most Common)

**Roles:**
- **Product Owner (PM)**: Defines what to build and prioritizes
- **Scrum Master**: Facilitates process and removes blockers
- **Development Team**: Builds the product

**Artifacts:**
- **Product Backlog**: Prioritized list of all work
- **Sprint Backlog**: Work committed for current sprint
- **Increment**: Potentially shippable product at sprint end

**Events:**
- Sprint Planning
- Daily Standup
- Sprint Review
- Sprint Retrospective

**Sprint Length:** Typically 1-2 weeks

---

### Kanban

**Key Concepts:**
- **Continuous flow** (no fixed sprints)
- **Visual board** (To Do, In Progress, Done)
- **WIP limits** (limit work in progress)
- **Pull system** (team pulls work when ready)

**Best for:**
- Support/maintenance teams
- Continuous delivery environments
- Teams wanting more flexibility than Scrum

---

## The Agile Sprint Cycle

### Week 0: Preparation
```
[ ] Backlog grooming
[ ] Stories estimated
[ ] Stories prioritized
[ ] Team capacity known
[ ] Dependencies identified
```

### Week 1: Sprint Start
```
Day 1: Sprint Planning
Days 2-5: Development + Daily Standups
```

### Week 2: Sprint End
```
Days 1-4: Development + Daily Standups
Day 5: Sprint Review + Retrospective
```

---

## Sprint Planning Deep Dive

### Before Sprint Planning

**Product Manager Preparation:**
- Top backlog items are detailed
- User stories have acceptance criteria
- Designs are ready if needed
- Dependencies are identified
- Business value is clear

**Team Preparation:**
- Review upcoming stories
- Technical questions noted
- Rough estimates ready

### During Sprint Planning (Part 1)

**Duration:** 1-2 hours

**Agenda:**
1. Review sprint goal
2. PM presents prioritized stories
3. Team asks clarifying questions
4. Team selects stories for sprint
5. Confirm sprint commitment

**Output:** Draft sprint backlog

### During Sprint Planning (Part 2)

**Duration:** 1-2 hours

**Agenda:**
1. Break down stories into tasks
2. Estimate tasks in hours
3. Identify technical approach
4. Assign initial owners
5. Confirm capacity vs. commitment

**Output:** Detailed sprint plan

---

## Daily Standup Format

**Time:** 15 minutes maximum
**When:** Same time every day
**Who:** Entire team (PM, developers, designers, QA)

### The Three Questions

Each team member answers:
1. **What did I do yesterday?**
2. **What will I do today?**
3. **Are there any blockers?**

### PM's Role in Standup

**Listen for:**
- Scope creep or confusion
- Blocked team members
- Stories taking longer than expected
- Need for clarification

**After Standup:**
- Immediately address blockers
- Follow up with individuals as needed
- Update stakeholders if issues affect timeline

---

## Backlog Management

### User Story Priority

**Must Have (P0):**
- Critical business needs
- Regulatory requirements
- Severe bugs

**Should Have (P1):**
- Important features
- Significant improvements
- Major bugs

**Nice to Have (P2):**
- Enhancement requests
- Minor bugs
- Technical debt

**Won't Have (This Sprint):**
- Low priority items
- Future considerations
- Deferred requests

### Story Readiness Checklist

A story is ready when it has:
- [ ] Clear title and description
- [ ] User story format ("As a... I want... So that...")
- [ ] Acceptance criteria
- [ ] Designs (if UI work)
- [ ] Technical feasibility confirmed
- [ ] Dependencies identified
- [ ] Estimated by team
- [ ] Priority assigned

---

## Estimation Techniques

### Story Points (Recommended)

**Fibonacci Scale:** 1, 2, 3, 5, 8, 13, 21

- **1 point**: Trivial change (few hours)
- **2 points**: Simple story (1 day)
- **3 points**: Straightforward (1-2 days)
- **5 points**: Moderate complexity (2-3 days)
- **8 points**: Complex (3-5 days)
- **13 points**: Very complex (full week)
- **21+ points**: Too large, should be split

### Planning Poker

1. PM reads user story
2. Team discusses and asks questions
3. Each person selects estimate card
4. All reveal simultaneously
5. Discuss differences
6. Re-estimate until consensus

### T-Shirt Sizing

For rough estimates:
- **XS**: Trivial
- **S**: Small
- **M**: Medium
- **L**: Large
- **XL**: Extra Large (should be split)

---

## Sprint Review (Demo)

### Preparation

**Before the Meeting:**
- [ ] Ensure demo environment is ready
- [ ] Test all features to demo
- [ ] Prepare talking points
- [ ] Invite stakeholders
- [ ] Set up screen sharing

### Meeting Structure

**Duration:** 1-2 hours

**Agenda:**
1. **Sprint Goal Review** (5 min)
   - What we set out to achieve
   
2. **Demo Completed Work** (30-45 min)
   - Show each completed story
   - Demonstrate functionality
   - Explain business value
   
3. **Metrics & Data** (10 min)
   - Velocity
   - Completion rate
   - Quality metrics
   
4. **What Didn't Get Done** (5 min)
   - Uncompleted stories
   - Reasons and learnings
   
5. **Stakeholder Feedback** (15-20 min)
   - Questions
   - Concerns
   - Additional requirements
   
6. **Next Sprint Preview** (10 min)
   - Upcoming priorities
   - Expected outcomes

---

## Sprint Retrospective

### Format: Start, Stop, Continue

**Start:** What should we start doing?
- New practices
- Tools or processes
- Communication methods

**Stop:** What should we stop doing?
- Ineffective practices
- Time wasters
- Obstacles

**Continue:** What should we keep doing?
- Successful practices
- Effective tools
- Good habits

### Alternative Formats

**Mad, Sad, Glad:**
- Mad: What frustrated us?
- Sad: What disappointed us?
- Glad: What made us happy?

**Four Ls:**
- Liked: What did we enjoy?
- Learned: What did we learn?
- Lacked: What was missing?
- Longed for: What do we wish we had?

**Sailboat:**
- Wind: What helped us?
- Anchor: What held us back?
- Rocks: What risks do we face?
- Island: What's our goal?

### Action Items

**Every retrospective should produce 1-3 action items:**
- Specific and measurable
- Assigned to an owner
- Due date set
- Tracked in next retrospective

---

## Managing Sprint Scope

### When New Work Appears

**Critical Bug:**
- Assess severity
- If critical: add to sprint, remove equivalent work
- If not critical: add to backlog

**Urgent Stakeholder Request:**
- Evaluate: Is it truly urgent?
- What's the business impact of waiting?
- What would need to be removed?
- Make data-driven decision

**Scope Creep:**
- Recognize it early
- Discuss with team
- Options:
  1. Defer to next sprint
  2. Reduce scope of current story
  3. Accept sprint goal won't be met

### When Work Is Blocked

**PM Actions:**
1. Identify the blocker
2. Assess impact on sprint goal
3. Options:
   - Pull in another story
   - Work on next sprint items
   - Technical debt/improvements
4. Remove the blocker ASAP

---

## Measuring Agile Success

### Team Velocity

**What it is:** Average story points completed per sprint

**How to calculate:**
```
Sprint 1: 21 points
Sprint 2: 25 points
Sprint 3: 23 points
Average Velocity: 23 points
```

**Use it for:**
- Sprint planning
- Release planning
- Capacity forecasting

**Don't use it for:**
- Comparing teams
- Performance evaluation
- Rigid commitments

### Sprint Burndown

**X-axis:** Days in sprint
**Y-axis:** Remaining story points

**Ideal:** Steady downward slope
**Reality:** Often erratic, but trending down

**Red flags:**
- Flat line (no progress)
- Upward trend (scope increasing)
- Sudden drop at end (poor estimates)

### Team Health Metrics

- **Sprint Goal Achievement**: % of sprints meeting goal
- **Commitment Reliability**: Completed vs. committed points
- **Bug Escape Rate**: Bugs found in production
- **Cycle Time**: Idea to production duration
- **Team Happiness**: Regular team surveys

---

## Common Agile Challenges

### Challenge: Stories not finished by sprint end
**Solutions:**
- Improve estimation
- Break down stories smaller
- Address blockers faster
- Reduce work in progress

### Challenge: Unclear requirements
**Solutions:**
- Better acceptance criteria
- More grooming time
- Involve team earlier
- Use examples and mockups

### Challenge: Scope creep
**Solutions:**
- Protect sprint commitment
- Have strong sprint goal
- Defer non-urgent work
- Educate stakeholders

### Challenge: Low team morale
**Solutions:**
- Listen in retrospectives
- Act on feedback
- Celebrate wins
- Address burnout

---

## Agile Best Practices

### For Product Managers

1. **Write clear stories** with acceptance criteria
2. **Prioritize ruthlessly** based on value
3. **Be available** to answer questions
4. **Trust the team** to estimate and commit
5. **Protect the team** from external pressure
6. **Celebrate successes** at sprint reviews
7. **Act on retrospectives** to improve continuously

### For Teams

1. **Keep standups focused** (15 min max)
2. **Update stories regularly** so PM knows status
3. **Ask questions early** don't wait until standup
4. **Help teammates** who are blocked
5. **Test as you go** don't leave it for the end
6. **Speak up in retrospectives** share honest feedback
7. **Take estimation seriously** it affects planning

---

## Agile at Scale

### Multiple Teams

**Approaches:**
- **Scrum of Scrums**: Representatives from each team meet
- **SAFe**: Scaled Agile Framework with multiple layers
- **LeSS**: Large-Scale Scrum with simpler structure

**PM Coordination:**
- Align roadmaps across teams
- Manage dependencies
- Synchronized sprints can help
- Shared backlog or separate backlogs

### Large Features

**Epics:** Large features spanning multiple sprints
- Break into smaller stories
- Deliver incrementally
- Show progress each sprint
- Can span multiple teams

---

## Tools for Agile Teams

### Project Management
- Jira
- Azure DevOps
- Linear
- Clubhouse/Shortcut

### Sprint Board
- Physical board (sticky notes)
- Digital board (Jira, Trello)
- Kanban tools (Kanbanize)

### Estimation
- Planning Poker apps
- Pointing Poker
- Scrum Poker

---

## Resources

- [Agile Manifesto](https://agilemanifesto.org/)
- [Scrum Guide](https://scrumguides.org/)
- [Atlassian Agile Coach](https://www.atlassian.com/agile)
- [Mountain Goat Software Blog](https://www.mountaingoatsoftware.com/blog)
