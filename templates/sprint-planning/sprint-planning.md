# Sprint Planning Template

## Sprint Information

**Sprint Number:** [X]  
**Sprint Goal:** [One clear sentence describing what the sprint aims to achieve]  
**Sprint Duration:** [Start Date] to [End Date] ([X] weeks)  
**Team Capacity:** [X] story points or [Y] person-days

---

## Sprint Planning Meeting

**Date:** [Date]  
**Duration:** [X] hours  
**Attendees:**
- Product Manager: [Name]
- Scrum Master: [Name]
- Engineering Team: [Names]
- Designer: [Name] (if needed)

---

## Part 1: Sprint Goal & Story Selection (1-2 hours)

### Sprint Goal

**Primary Objective:**
[What is the main thing we want to accomplish this sprint?]

**Success Criteria:**
- [ ] [Measurable outcome 1]
- [ ] [Measurable outcome 2]

**Why This Matters:**
[Business value, user impact, or strategic importance]

---

### Backlog Review

#### Selected Stories

| Story ID | Story Title | Story Points | Priority | Assignee | Dependencies |
|----------|-------------|--------------|----------|----------|--------------|
| [ID-001] | [Title] | 8 | P0 | [Name] | None |
| [ID-002] | [Title] | 5 | P1 | [Name] | ID-001 |
| [ID-003] | [Title] | 3 | P1 | [Name] | None |
| [ID-004] | [Title] | 5 | P2 | [Name] | None |

**Total Story Points:** [X]

---

#### Stories NOT Selected (For Next Sprint)

| Story ID | Story Title | Reason Deferred |
|----------|-------------|-----------------|
| [ID-005] | [Title] | Lower priority |
| [ID-006] | [Title] | Dependencies not ready |

---

### Capacity Planning

**Team Members:**

| Name | Availability | Capacity (Days) | Capacity (Points) |
|------|--------------|-----------------|-------------------|
| [Dev 1] | 100% | 10 days | 13 points |
| [Dev 2] | 80% (PTO) | 8 days | 10 points |
| [Dev 3] | 100% | 10 days | 13 points |
| [Designer] | 50% (shared) | 5 days | N/A |

**Total Team Capacity:** [X] points

**Committed:** [Y] points  
**Buffer:** [Z]% for unexpected work

---

## Part 2: Task Breakdown (1-2 hours)

### Story 1: [Story Title]

**Story Points:** [X]  
**Assigned To:** [Name]

**Tasks:**
- [ ] [Task 1] - [Estimated hours] - [Owner]
- [ ] [Task 2] - [Estimated hours] - [Owner]
- [ ] [Task 3] - [Estimated hours] - [Owner]
- [ ] [Task 4] - [Estimated hours] - [Owner]

**Technical Approach:**
[Brief description of how this will be implemented]

**Testing Requirements:**
- Unit tests: [Description]
- Integration tests: [Description]
- Manual testing: [Description]

---

### Story 2: [Story Title]

**Story Points:** [X]  
**Assigned To:** [Name]

**Tasks:**
- [ ] [Task 1] - [Estimated hours] - [Owner]
- [ ] [Task 2] - [Estimated hours] - [Owner]
- [ ] [Task 3] - [Estimated hours] - [Owner]

**Technical Approach:**
[Brief description]

---

## Dependencies & Blockers

### Internal Dependencies
- [ ] [Dependency 1] - **Status:** [Ready/Blocked/In Progress] - **Owner:** [Name]
- [ ] [Dependency 2] - **Status:** [Ready/Blocked/In Progress] - **Owner:** [Name]

### External Dependencies
- [ ] [External team/service] - **Status:** [Status] - **Contact:** [Name]
- [ ] [Third-party service] - **Status:** [Status] - **ETA:** [Date]

### Known Risks
- **Risk 1:** [Description] - **Mitigation:** [Plan]
- **Risk 2:** [Description] - **Mitigation:** [Plan]

---

## Definition of Done

A story is considered "done" when:

**Code:**
- [ ] Code written and follows style guidelines
- [ ] Code reviewed and approved by peer
- [ ] Unit tests written with >80% coverage
- [ ] Integration tests pass
- [ ] No critical or high bugs

**Documentation:**
- [ ] Code comments for complex logic
- [ ] API documentation updated
- [ ] User-facing documentation updated

**Quality:**
- [ ] Acceptance criteria met
- [ ] Tested in staging environment
- [ ] PM/PO approval obtained
- [ ] Accessible (WCAG AA)
- [ ] Performance acceptable

**Deployment:**
- [ ] Merged to main/release branch
- [ ] Deployed to production (or ready to deploy)
- [ ] Monitoring/alerts configured

---

## Sprint Commitments

### What We're Committing To:
- [Commitment 1]
- [Commitment 2]
- [Commitment 3]

### What We're NOT Committing To:
- [Stretch goal 1]
- [Nice-to-have 2]

### Confidence Level:
[High/Medium/Low] - [Explanation]

---

## Communication Plan

### Daily Standups
- **Time:** [Time]
- **Location:** [Room/Video link]
- **Duration:** 15 minutes

### Mid-Sprint Check-in
- **When:** [Day/Date]
- **Purpose:** Review progress, adjust if needed

### Sprint Review/Demo
- **When:** [Date/Time]
- **Attendees:** [List]
- **What to demo:** [Stories to demonstrate]

### Sprint Retrospective
- **When:** [Date/Time]
- **Facilitator:** [Name]

---

## Sprint Board Setup

### Columns:
1. **Backlog** - Stories selected for sprint
2. **To Do** - Ready to be worked on
3. **In Progress** - Actively being worked on
4. **In Review** - Code review / PR open
5. **Testing** - QA testing
6. **Done** - Meets definition of done

### WIP Limits:
- In Progress: Max [X] stories
- In Review: Max [Y] stories

---

## Questions & Clarifications

### Resolved During Planning:
- **Q:** [Question]  
  **A:** [Answer] - [Decided by]

- **Q:** [Question]  
  **A:** [Answer] - [Decided by]

### Open Questions (Need Resolution):
- [ ] **Q:** [Question] - **Owner:** [Name] - **Due:** [Date]
- [ ] **Q:** [Question] - **Owner:** [Name] - **Due:** [Date]

---

## Notes & Action Items

### Key Decisions Made:
1. [Decision 1]
2. [Decision 2]

### Action Items:
- [ ] [Action 1] - [Owner] - [Due date]
- [ ] [Action 2] - [Owner] - [Due date]

### Follow-up Needed:
- [Topic 1] - [Person to follow up]
- [Topic 2] - [Person to follow up]

---

## Example: Sprint 24 Planning

**Sprint Goal:** Enable guest checkout to reduce cart abandonment

**Sprint Duration:** Jan 15 - Jan 28 (2 weeks)  
**Team Capacity:** 23 story points

### Selected Stories

| Story ID | Story Title | Points | Priority |
|----------|-------------|--------|----------|
| SHOP-101 | Guest can enter shipping info | 8 | P0 |
| SHOP-102 | Guest can save shipping info for later | 5 | P1 |
| SHOP-103 | Order confirmation email for guests | 3 | P1 |
| SHOP-104 | Guest can create account post-purchase | 5 | P2 |

**Total:** 21 points (2 points buffer)

### Sprint Goal Success Criteria:
- [ ] Guest users can complete checkout without account
- [ ] Order confirmation sent to guest email
- [ ] No increase in payment errors
- [ ] Checkout time < 3 minutes

### Key Risks:
- **Payment gateway integration**: Mitigate by testing integration early in sprint
- **Email delivery issues**: Set up monitoring and use established email service

### Definition of Done Specific to This Sprint:
- [ ] Works on mobile and desktop
- [ ] Payment security audit passed
- [ ] Load tested with 100 concurrent users
- [ ] Marketing team briefed for announcement
