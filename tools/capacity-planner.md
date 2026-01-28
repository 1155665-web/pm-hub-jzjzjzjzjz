# Capacity Planning Tool

## Overview

This guide helps product managers plan team capacity and balance workload across sprints and quarters.

---

## Understanding Capacity

**Capacity** = Available time for productive work

**Not all time is productive time:**
- Meetings
- Email/communication
- Context switching
- Breaks
- Training
- Support/maintenance

**Rule of Thumb:**
Productive capacity ≈ 60-70% of total time

---

## Calculating Sprint Capacity

### Individual Capacity

**Formula:**
```
Individual Capacity = (Work Days - PTO - Meetings) × Points per Day
```

**Example:**
```
Sprint length: 10 days (2 weeks)
PTO: 0 days
Meetings: 2 hours/day = 2.5 days
Available: 10 - 0 - 2.5 = 7.5 days

If developer can complete 2 story points/day:
Capacity = 7.5 × 2 = 15 story points
```

---

### Team Capacity

**Formula:**
```
Team Capacity = Sum of all individual capacities
```

**Example Team:**

| Name | Sprint Days | PTO | Meetings | Available | Pts/Day | Capacity |
|------|-------------|-----|----------|-----------|---------|----------|
| Sarah | 10 | 0 | 2.5 | 7.5 | 2 | 15 |
| Mike | 10 | 2 | 2.5 | 5.5 | 2 | 11 |
| Alex | 10 | 0 | 3 | 7 | 1.5 | 10.5 |

**Total Team Capacity:** 36.5 story points

---

## Capacity Planning Template

### Sprint Capacity Worksheet

**Sprint:** [Number]  
**Dates:** [Start] - [End]  
**Sprint Length:** [X] days

---

**Team Member 1: [Name]**

| Item | Value |
|------|-------|
| Total sprint days | [X] |
| PTO/vacation | [X] days |
| Holidays | [X] days |
| Meetings (estimated) | [X] days |
| Training/other | [X] days |
| **Available days** | **[Y]** |
| Story points per day | [Z] |
| **Sprint capacity** | **[Y × Z]** |

---

**Team Member 2: [Name]**
[Same table structure]

---

**Team Summary**

| Team Member | Capacity (Points) | Availability % |
|-------------|-------------------|----------------|
| [Name 1] | [X] | [Y]% |
| [Name 2] | [X] | [Y]% |
| [Name 3] | [X] | [Y]% |
| **Total** | **[Sum]** | **[Avg]%** |

---

### Buffer Allocation

**Total Capacity:** [X] points

**Allocations:**
- **Planned work:** [Y] points ([Z]%)
- **Bug fixes:** [A] points ([B]%)
- **Tech debt:** [C] points ([D]%)
- **Buffer (unplanned):** [E] points ([F]%)

**Recommended Buffer:** 20% for unexpected work

---

## Capacity Factors

### Time Deductions

**Meetings:**
- Daily standup: 15 min × 10 days = 2.5 hours
- Sprint planning: 2 hours
- Sprint review: 1 hour
- Retrospective: 1 hour
- Backlog grooming: 1 hour
- **Total:** 7.5 hours = ~1 day

**Communication:**
- Email/Slack: 1 hour/day
- Code reviews: 30 min/day
- Questions/help: 30 min/day
- **Total:** 2 hours/day = 2.5 days

**Context Switching:**
- Multiple projects: -20% capacity
- Interruptions: -10% capacity
- Learning curve: -10% capacity

---

### Capacity Multipliers

**Team Maturity:**
- New team: 0.6× (40% reduction)
- Growing team: 0.8× (20% reduction)
- Mature team: 1.0× (baseline)
- High-performing: 1.2× (20% increase)

**Technical Debt:**
- Low debt: 1.0× (no impact)
- Medium debt: 0.9× (10% reduction)
- High debt: 0.7× (30% reduction)

**Codebase Familiarity:**
- New codebase: 0.6× (40% reduction)
- Somewhat familiar: 0.8× (20% reduction)
- Very familiar: 1.0× (baseline)

---

## Quarterly Capacity Planning

### Quarter Capacity Worksheet

**Quarter:** [Q1/Q2/Q3/Q4] [Year]  
**Sprints:** [X] sprints

---

**Team Size & Composition:**

| Role | Count | Capacity/Sprint | Total |
|------|-------|-----------------|-------|
| Senior Engineers | [X] | [Y] pts | [Z] pts |
| Mid Engineers | [X] | [Y] pts | [Z] pts |
| Junior Engineers | [X] | [Y] pts | [Z] pts |
| **Total** | **[X]** | - | **[Sum]** |

**Per Sprint Capacity:** [X] points  
**Sprints in Quarter:** [Y]  
**Total Quarter Capacity:** [X × Y] points

---

**Time Off Planning:**

| Month | Holidays | Avg PTO | Impact (Days) | Impact (%) |
|-------|----------|---------|---------------|------------|
| [Month 1] | [X] days | [Y] days | [Z] days | [P]% |
| [Month 2] | [X] days | [Y] days | [Z] days | [P]% |
| [Month 3] | [X] days | [Y] days | [Z] days | [P]% |

**Adjusted Quarter Capacity:** [Original × (1 - Avg Impact%)]

---

**Allocation:**

| Category | Points | % of Total |
|----------|--------|------------|
| Features (new work) | [X] | [Y]% |
| Maintenance | [X] | [Y]% |
| Bug fixes | [X] | [Y]% |
| Technical debt | [X] | [Y]% |
| Improvements | [X] | [Y]% |
| R&D / Innovation | [X] | [Y]% |
| **Total** | **[Sum]** | **100%** |

**Recommended Allocation:**
- Features: 60-70%
- Maintenance: 10-15%
- Bug fixes: 5-10%
- Tech debt: 10-20%
- Improvements: 5-10%

---

## Balancing Capacity

### The 70-20-10 Rule

**70%** - Core product work
- New features
- Major improvements
- Roadmap items

**20%** - Sustaining activities
- Bug fixes
- Technical debt
- Performance optimization
- Security updates

**10%** - Innovation/Learning
- Experiments
- R&D
- New technology exploration
- Skill development

---

### Capacity Allocation by Team

**Feature Teams:**
- New features: 70-80%
- Tech debt: 10-15%
- Bugs: 10-15%

**Platform Teams:**
- Infrastructure: 60%
- Tech debt: 20%
- Support: 20%

**Sustaining Teams:**
- Bugs: 50%
- Maintenance: 30%
- Small improvements: 20%

---

## Capacity Planning Best Practices

### DO:
✅ **Plan conservatively** (better to under-promise)  
✅ **Include buffer** (20% for unexpected)  
✅ **Account for meetings** (they add up!)  
✅ **Track actual vs planned** (improve estimates)  
✅ **Adjust for holidays** (especially Q4)  
✅ **Consider team changes** (hiring, attrition)  
✅ **Balance work types** (features, bugs, debt)  
✅ **Review regularly** (capacity changes)  

### DON'T:
❌ **Assume 100% utilization** (unrealistic)  
❌ **Ignore meetings and overhead** (significant time)  
❌ **Over-allocate** (leads to burnout)  
❌ **Forget about PTO** (people need breaks)  
❌ **Neglect tech debt** (compounds over time)  
❌ **Plan sprint-to-sprint only** (need long view)  
❌ **Ignore velocity trends** (use historical data)  

---

## Handling Capacity Constraints

### When Capacity < Demand

**Options:**

**1. Reduce Scope**
- Prioritize ruthlessly
- Cut nice-to-haves
- Simplify features
- Move items to backlog

**2. Increase Capacity**
- Hire (takes time)
- Contract help
- Reduce meetings
- Improve efficiency
- Reduce context switching

**3. Extend Timeline**
- Push deadlines
- Phased rollout
- MVP first approach

**4. Improve Efficiency**
- Automate repetitive tasks
- Reduce technical debt
- Better tooling
- Pair programming for complex work

---

### When Capacity > Demand

**What to do with extra capacity:**

**1. Technical Debt**
- Refactoring
- Performance optimization
- Code cleanup
- Update dependencies

**2. Quality Improvements**
- Increase test coverage
- Fix long-standing bugs
- Improve documentation
- Accessibility improvements

**3. Innovation Time**
- Explore new technologies
- Build prototypes
- Hackathons
- Learning time

**4. Process Improvements**
- Improve CI/CD
- Better monitoring
- Dev tools
- Automation

---

## Capacity Tracking

### Track These Metrics

**Planned vs Actual:**
- Planned capacity: [X] points
- Actual completed: [Y] points
- Utilization: [Y/X × 100]%

**Capacity Breakdown:**
- Features: [X]% of capacity
- Bugs: [Y]% of capacity
- Tech debt: [Z]% of capacity
- Unplanned: [W]% of capacity

**Trends:**
- Average velocity: [X] points/sprint
- Trending up/down/stable
- Seasonal patterns
- Team changes impact

---

### Capacity Dashboard Template

**Sprint [X] Capacity Report**

**Planned:**
- Total capacity: [X] points
- Feature work: [Y] points
- Other work: [Z] points

**Actual:**
- Completed: [X] points
- Utilization: [Y]%
- Unplanned work: [Z] points

**Analysis:**
- [What went well]
- [What impacted capacity]
- [Adjustments for next sprint]

---

## Capacity Planning Tools

### Spreadsheets
- Google Sheets
- Excel
- Airtable

### Project Management
- Jira (capacity planning features)
- Linear (capacity views)
- Asana (workload view)
- Monday.com

### Specialized Tools
- Forecast
- Resource Guru
- Float
- Teamwork

---

## Example: Quarter Planning

**Q1 2024 Capacity Plan**

**Team:** 6 engineers

**Sprint Capacity:**
- Average per sprint: 45 points
- Sprints in Q1: 6
- Total Q1 capacity: 270 points

**Adjustments:**
- New Year holiday: -3% (8 points)
- Team member on leave: -5% (14 points)
- Adjusted capacity: 248 points

**Allocation:**
- Features (65%): 161 points
- Tech debt (20%): 50 points
- Bugs (10%): 25 points
- Buffer (5%): 12 points

**Major Features Planned:**
- Guest checkout: 42 points (2.5 sprints)
- Mobile redesign: 65 points (4 sprints)
- Payment optimization: 38 points (2 sprints)
- Small features: 16 points

**Total:** 161 points (matches allocation)

**Confidence:** Medium-High
- Team stable
- Features well-defined
- Reasonable buffer

---

## Resources

- [Capacity Planning Guide](https://www.atlassian.com/agile/project-management/capacity-planning)
- [Sprint Planning](https://www.scrum.org/resources/what-is-sprint-planning)
- [Resource Management](https://www.forecast.app/blog/capacity-planning)
