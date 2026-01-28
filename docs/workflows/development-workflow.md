# Development Workflow Guide

## Overview

This guide outlines the standard development workflow for product teams, helping product managers understand and coordinate with engineering.

## The Software Development Lifecycle

```
Product Discovery → Design → Development → Testing → Deployment → Monitoring
         ↑                                                              ↓
         └──────────────────── Feedback Loop ─────────────────────────┘
```

## Workflow Stages

### 1. Product Discovery

**PM Activities:**
- User research and interviews
- Market analysis
- Competitor research
- Problem validation
- Solution ideation

**Deliverables:**
- Problem statement
- User personas
- Customer journey maps
- Opportunity sizing

**Duration:** 1-4 weeks depending on complexity

---

### 2. Requirements & Design

**PM Activities:**
- Write user stories
- Define acceptance criteria
- Create wireframes/mockups
- Prioritize features
- Technical feasibility assessment

**Collaboration Points:**
- Design review with UX team
- Technical review with engineering
- Stakeholder alignment

**Deliverables:**
- Product requirements document (PRD)
- User stories with acceptance criteria
- Design mockups
- Success metrics definition

**Duration:** 1-2 weeks

---

### 3. Sprint Planning

**PM Activities:**
- Present backlog items
- Clarify requirements
- Answer questions
- Prioritize sprint scope
- Agree on sprint goals

**Engineering Activities:**
- Estimate story points
- Identify technical dependencies
- Break down tasks
- Commit to sprint capacity

**Output:**
- Sprint backlog
- Sprint goal
- Definition of done

**Duration:** 2-4 hours for 2-week sprint

---

### 4. Development

**PM Activities:**
- Daily standups
- Answer clarifying questions
- Review work in progress
- Unblock team members
- Manage scope changes

**Engineering Activities:**
- Write code
- Code reviews
- Unit testing
- Integration testing
- Documentation

**Best Practices:**
- Keep communication channels open
- Review work frequently (not just at end)
- Be available for questions
- Protect team from scope creep

**Duration:** Sprint length (typically 1-2 weeks)

---

### 5. Quality Assurance

**PM Activities:**
- Provide test scenarios
- Review test cases
- Participate in testing
- Validate acceptance criteria
- Sign off on features

**QA Activities:**
- Write test cases
- Execute test plans
- Report bugs
- Regression testing
- Performance testing

**Acceptance Criteria:**
- All functionality works as specified
- No critical or high-priority bugs
- Performance meets requirements
- Security checks passed

**Duration:** Overlaps with development, continues through sprint

---

### 6. Sprint Review/Demo

**PM Activities:**
- Demonstrate completed features
- Gather feedback
- Update roadmap
- Celebrate successes

**Attendees:**
- Product team
- Engineering team
- Stakeholders
- Customers (optional)

**Agenda:**
1. Review sprint goal
2. Demo completed features
3. Discuss metrics
4. Get feedback
5. Preview next sprint

**Duration:** 1-2 hours

---

### 7. Deployment

**PM Activities:**
- Review deployment plan
- Approve production release
- Prepare release notes
- Communicate to stakeholders
- Plan rollback if needed

**Deployment Strategies:**

**Big Bang:** Deploy everything at once
- Pros: Simple, fast
- Cons: Risky, hard to rollback

**Phased Rollout:** Deploy to subset of users
- Pros: Lower risk, can test with real users
- Cons: More complex, longer timeline

**Feature Flags:** Deploy code but enable for specific users
- Pros: Easy rollback, A/B testing
- Cons: Technical complexity

**Blue-Green:** Maintain two environments, switch traffic
- Pros: Zero downtime, easy rollback
- Cons: Infrastructure cost

**Duration:** Minutes to days depending on strategy

---

### 8. Monitoring & Feedback

**PM Activities:**
- Monitor key metrics
- Gather user feedback
- Track issues/bugs
- Measure success criteria
- Plan iterations

**Metrics to Track:**
- Usage metrics (adoption, engagement)
- Performance metrics (speed, uptime)
- Business metrics (conversion, revenue)
- User satisfaction (NPS, surveys)

**Tools:**
- Analytics platforms (Mixpanel, Amplitude)
- Error tracking (Sentry, Rollbar)
- User feedback (Intercom, UserVoice)
- APM (New Relic, Datadog)

**Duration:** Ongoing

---

### 9. Sprint Retrospective

**Purpose:** Continuous improvement

**Format:**
1. What went well?
2. What could be improved?
3. Action items for next sprint

**PM Role:**
- Facilitate discussion
- Document insights
- Ensure action items are tracked
- Follow up on previous action items

**Duration:** 45-60 minutes

---

## Daily Workflows

### Product Manager's Daily Routine

**Morning:**
- Check overnight metrics/alerts
- Review customer feedback
- Prepare for standup
- Respond to urgent questions

**Standup (Daily):**
- Listen to team updates
- Note blockers
- Answer questions
- Adjust priorities if needed

**Throughout Day:**
- Answer team questions
- Review work in progress
- Stakeholder communication
- Work on next sprint items
- Bug triage

**End of Day:**
- Update roadmap/backlog
- Document decisions
- Respond to feedback
- Plan tomorrow's priorities

---

## Common Development Practices

### Version Control (Git)

**Branching Strategy:**
```
main (production)
  ├── develop (integration)
  │   ├── feature/user-authentication
  │   ├── feature/payment-integration
  │   └── bugfix/login-error
```

**PM Involvement:**
- Understand branch structure
- Review pull requests
- Track feature branches
- Approve merges to main

### Code Review Process

1. Developer creates pull request (PR)
2. Automated tests run
3. Peer review by other developers
4. PM review (optional but recommended)
5. Merge to main branch

**PM Code Review Tips:**
- Focus on functionality, not code quality
- Verify acceptance criteria are met
- Check error messages and edge cases
- Ensure user experience matches design

### Continuous Integration/Continuous Deployment (CI/CD)

**Pipeline Stages:**
```
Commit → Build → Test → Stage → Deploy → Monitor
```

**PM Checkpoints:**
- Staging environment: Review before production
- Production deployment: Monitor metrics
- Rollback plan: Understand rollback process

---

## Agile Ceremonies

### Daily Standup (15 min)
- **When:** Every morning
- **Who:** Development team, PM, Scrum Master
- **Format:** Each person shares: Yesterday, Today, Blockers

### Sprint Planning (2-4 hours)
- **When:** Start of each sprint
- **Who:** Full team
- **Output:** Sprint backlog and goals

### Sprint Review (1-2 hours)
- **When:** End of sprint
- **Who:** Team + stakeholders
- **Output:** Feedback and acceptance

### Sprint Retrospective (45-60 min)
- **When:** End of sprint
- **Who:** Development team
- **Output:** Improvement action items

### Backlog Refinement (1-2 hours)
- **When:** Mid-sprint
- **Who:** PM, Tech Lead, key developers
- **Output:** Estimated and ready stories

---

## Communication Patterns

### Synchronous Communication
- Standups: Quick updates
- Slack/Teams: Urgent questions
- Video calls: Complex discussions
- In-person: Sensitive topics

### Asynchronous Communication
- Jira/Linear: Requirements and updates
- Documents: Detailed specifications
- Email: Stakeholder updates
- Recorded demos: Feature showcases

---

## Tools & Platforms

### Project Management
- **Jira**: Enterprise teams
- **Linear**: Tech-focused teams
- **Asana**: Cross-functional teams
- **Trello**: Simple projects

### Documentation
- **Confluence**: Wiki-style docs
- **Notion**: All-in-one workspace
- **Google Docs**: Collaborative writing
- **GitHub/GitLab**: Technical docs with code

### Communication
- **Slack**: Team messaging
- **Microsoft Teams**: Enterprise communication
- **Zoom/Meet**: Video conferencing

### Design
- **Figma**: UI/UX design
- **Miro**: Whiteboarding
- **Lucidchart**: Diagrams and flowcharts

---

## Best Practices for Product Managers

### 1. Write Clear Requirements
- Use user story format: "As a [user], I want [goal], so that [benefit]"
- Include acceptance criteria
- Add examples and edge cases
- Attach mockups/wireframes

### 2. Maintain the Backlog
- Keep top items detailed and ready
- Prioritize ruthlessly
- Remove outdated items
- Regular grooming sessions

### 3. Be Available
- Respond quickly to questions
- Attend standups consistently
- Review work in progress
- Unblock team members

### 4. Understand Technical Constraints
- Learn basic technical concepts
- Understand architecture
- Know the tech stack
- Appreciate complexity

### 5. Measure Success
- Define metrics upfront
- Track continuously
- Share results regularly
- Learn and iterate

---

## Common Challenges & Solutions

### Challenge: Requirements changing mid-sprint
**Solution:** 
- Evaluate urgency vs. impact
- If critical: adjust sprint scope
- If not: add to next sprint
- Document and communicate changes

### Challenge: Features not meeting acceptance criteria
**Solution:**
- Review criteria during development
- Provide feedback early
- Clear definition of done
- Accept technical debt if needed

### Challenge: Team velocity unpredictable
**Solution:**
- Track historical velocity
- Account for team changes
- Buffer in planning
- Improve estimation over time

### Challenge: Stakeholder pressure for more features
**Solution:**
- Show capacity constraints
- Prioritize based on value
- Say no to less important items
- Manage expectations proactively

---

## Resources

- [Agile Manifesto](https://agilemanifesto.org/)
- [Scrum Guide](https://scrumguides.org/)
- [Product Management Resources](https://www.productplan.com/learn/)
