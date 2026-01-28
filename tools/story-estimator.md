# User Story Estimator Guide

## Overview

This guide helps product managers and development teams estimate user stories effectively using story points and other estimation techniques.

---

## What are Story Points?

Story points are a unit of measure for expressing the overall effort required to implement a user story.

**Story points measure:**
- Complexity
- Amount of work
- Uncertainty/risk
- Knowledge required

**Story points DON'T measure:**
- Exact hours or days
- Individual developer speed
- Calendar time

---

## Common Estimation Scales

### Fibonacci Sequence (Recommended)

**1, 2, 3, 5, 8, 13, 21**

- **1 point:** Trivial, well-understood, few hours
- **2 points:** Simple, straightforward, 1 day
- **3 points:** Moderate complexity, 1-2 days
- **5 points:** Average complexity, 2-3 days
- **8 points:** Complex, 3-5 days, some unknowns
- **13 points:** Very complex, needs breakdown
- **21+ points:** Epic, must be split

**Why Fibonacci?**
- Larger gaps reflect increasing uncertainty
- Forces meaningful distinctions
- Industry standard

---

### T-Shirt Sizes

**XS, S, M, L, XL**

**When to use:**
- Initial rough estimates
- Very early planning
- Non-technical stakeholders
- Portfolio-level planning

**Conversion to Fibonacci:**
- XS = 1-2 points
- S = 3 points
- M = 5 points
- L = 8 points
- XL = 13+ points (needs splitting)

---

## Estimation Techniques

### 1. Planning Poker

**Most popular and effective technique**

**How it works:**
1. Product manager reads user story
2. Team discusses and asks questions
3. Each person privately selects estimate card
4. All reveal simultaneously
5. Discuss outliers (highest and lowest)
6. Re-estimate until consensus (or average)

**Benefits:**
- Democratic and engaging
- Surfaces assumptions
- Creates shared understanding
- More accurate than individual estimates

**Tools:**
- Physical cards
- Planning Poker apps
- Zoom polls

---

### 2. Relative Sizing

**Compare stories to baseline stories**

**Process:**
1. Select a "reference story" (e.g., 5 points)
2. For each new story, ask:
   - Simpler or more complex than reference?
   - By how much?
3. Assign points relative to reference

**Example:**
```
Reference Story (5 pts): Add email validation to login

New Story: Add password strength meter
→ Similar complexity = 5 points

New Story: Implement OAuth login
→ Much more complex = 13 points

New Story: Fix typo in error message
→ Much simpler = 1 point
```

---

### 3. Bucket System

**Good for estimating large backlogs**

**Setup:**
Create buckets labeled: 1, 2, 3, 5, 8, 13, 21

**Process:**
1. Read story aloud
2. Quick discussion (2 min max)
3. Place in appropriate bucket
4. Move on to next story

**Benefits:**
- Fast (can estimate 50+ stories/hour)
- Relative sizing built-in
- Good for backlog refinement

---

### 4. Three-Point Estimation

**For more precision when needed**

**Estimate three scenarios:**
- **Best case** (optimistic)
- **Most likely** (realistic)
- **Worst case** (pessimistic)

**Formula:**
```
Estimate = (Best + 4×Most Likely + Worst) / 6
```

**Example:**
```
Best case: 2 days
Most likely: 5 days
Worst case: 10 days

Estimate = (2 + 4×5 + 10) / 6 = 32/6 = 5.3 days
```

**When to use:**
- Critical features
- High uncertainty
- Need confidence intervals
- Executive reporting

---

## Estimation Guidelines by Complexity

### 1 Point: Trivial

**Characteristics:**
- Very well understood
- Minimal code changes
- No dependencies
- < 4 hours work

**Examples:**
- Update text on button
- Change color of element
- Fix typo
- Add simple validation
- Update copy in email

---

### 2 Points: Simple

**Characteristics:**
- Straightforward implementation
- Familiar territory
- Few unknowns
- ~1 day work

**Examples:**
- Add field to form
- Create simple API endpoint
- Basic CRUD operation
- Simple UI component
- Write unit tests for feature

---

### 3 Points: Moderate

**Characteristics:**
- Some complexity
- Mostly understood
- Minor unknowns
- 1-2 days work

**Examples:**
- Form with validation
- Filter or search feature
- Simple authentication
- Dashboard widget
- Integration with known API

---

### 5 Points: Average

**Characteristics:**
- Moderate complexity
- Some research needed
- Multiple components affected
- 2-3 days work

**Examples:**
- User profile page
- File upload with preview
- Email notification system
- Report generation
- Third-party integration

---

### 8 Points: Complex

**Characteristics:**
- High complexity
- Significant unknowns
- Multiple systems involved
- 3-5 days work

**Examples:**
- Payment gateway integration
- Advanced search with filters
- Real-time notifications
- Multi-step wizard
- Data migration script

---

### 13 Points: Very Complex

**Characteristics:**
- Very high complexity
- Many unknowns
- Cross-team coordination
- Full week or more

**Examples:**
- Authentication system
- Admin dashboard
- Analytics implementation
- Major refactoring
- Complex algorithm

**Recommendation:** Consider splitting into smaller stories

---

### 21+ Points: Too Large

**Don't estimate stories this large**

Instead:
- Break into smaller stories
- Create an epic
- Do spike/research first
- Refine until < 13 points

---

## Factors That Affect Estimates

### Complexity Factors

**Code Complexity:**
- Algorithm complexity
- Number of edge cases
- Business logic intricacy

**Technical Complexity:**
- New technology/framework
- Performance requirements
- Security considerations
- Scalability needs

**Integration Complexity:**
- Number of systems involved
- API dependencies
- Data transformations

---

### Uncertainty Factors

**Requirements Uncertainty:**
- Vague acceptance criteria
- Unclear edge cases
- Changing requirements

**Technical Uncertainty:**
- New technology
- Unknown feasibility
- Performance unknowns

**Team Uncertainty:**
- Unfamiliar codebase
- New team members
- Knowledge gaps

---

### Effort Factors

**Development Effort:**
- Lines of code
- Number of files
- Test coverage needed

**Related Work:**
- Design needed
- Documentation
- Testing
- Code review
- Deployment

---

## Estimation Template

### Story Estimation Worksheet

**Story Title:** [Title]

**User Story:**
As a [user], I want [goal], so that [benefit]

---

**Complexity Assessment:**

| Factor | Rating (1-5) | Notes |
|--------|--------------|-------|
| Code complexity | [ ] | [Details] |
| Technical complexity | [ ] | [Details] |
| Integration needs | [ ] | [Details] |
| Uncertainty | [ ] | [Details] |
| Amount of work | [ ] | [Details] |

**Total Complexity Score:** [Sum] / 25

---

**Reference Comparisons:**

Similar to: [Previous story] ([X] points)  
Simpler than: [Previous story] ([Y] points)  
More complex than: [Previous story] ([Z] points)

---

**Team Discussion Notes:**
- [Key point 1]
- [Key point 2]
- [Question 1]

---

**Estimated Size:** [Points]

**Confidence Level:** [High/Medium/Low]

**Assumptions:**
- [Assumption 1]
- [Assumption 2]

**Risks:**
- [Risk 1]
- [Risk 2]

---

## Estimation Best Practices

### DO:
✅ **Estimate as a team** (not just one person)  
✅ **Use reference stories** for consistency  
✅ **Include all work** (dev, test, review, docs)  
✅ **Re-estimate** if requirements change  
✅ **Track velocity** to improve estimates  
✅ **Break down large stories** (> 13 points)  
✅ **Discuss outliers** when estimates vary  
✅ **Consider the team** (their skills and experience)  

### DON'T:
❌ **Convert to hours** (defeats the purpose)  
❌ **Compare team velocities** (each team unique)  
❌ **Use estimates for performance reviews**  
❌ **Let one person dominate** estimation  
❌ **Rush the process** (takes time)  
❌ **Ignore unknowns** (factor in uncertainty)  
❌ **Estimate until requirements clear**  
❌ **Feel pressured** to lowball estimates  

---

## Handling Difficult Scenarios

### Scenario: Team Can't Agree on Estimate

**What to do:**
1. Have highest and lowest explain reasoning
2. Clarify requirements if needed
3. Identify assumptions
4. Consider splitting story
5. If still stuck, go with higher estimate (safer)
6. Add note to revisit after spike

---

### Scenario: Story Has Too Many Unknowns

**What to do:**
1. Create a spike story for research
2. Estimate spike (usually 2-5 points)
3. Timebox the spike (1-2 days)
4. Re-estimate original story after spike
5. Document learnings

---

### Scenario: Estimates Always Wrong

**What to do:**
1. Track actual vs. estimated
2. Identify patterns (always over/under?)
3. Adjust baseline understanding
4. More detailed acceptance criteria
5. Break stories down smaller
6. Improve definition of done

---

### Scenario: New Team Member

**What to do:**
1. They should participate but not vote initially
2. Learn from team discussions
3. Start voting after 2-3 sessions
4. Adjust team velocity temporarily
5. Mentor them on estimation

---

## Velocity Tracking

### Calculate Team Velocity

**Formula:**
```
Velocity = Story points completed in sprint
```

**Track over time:**
```
Sprint 1: 18 points
Sprint 2: 22 points
Sprint 3: 20 points
Sprint 4: 24 points
Average: 21 points
```

**Use velocity for:**
- Sprint planning (don't over-commit)
- Release planning (forecast completion)
- Identifying trends
- Setting expectations

**Don't use velocity for:**
- Comparing teams
- Performance reviews
- Rigid commitments
- External reporting

---

## Estimation Anti-Patterns

### The "That's Easy" Trap

**Problem:** Underestimating because it "seems easy"

**Solution:** 
- Always discuss edge cases
- Include testing, review, docs
- Ask: "What could go wrong?"
- Consider full scope

---

### The "We'll Figure It Out" Trap

**Problem:** Estimating despite major unknowns

**Solution:**
- Do a spike first
- Increase estimate for uncertainty
- Break down and estimate pieces
- Get more requirements

---

### The "Pressure to Commit" Trap

**Problem:** Lowering estimates due to pressure

**Solution:**
- Stick to honest estimates
- Explain risks of underestimating
- Show historical accuracy
- Educate stakeholders

---

## Estimation Checklist

**Before Estimating:**
- [ ] User story clearly written
- [ ] Acceptance criteria defined
- [ ] Designs available (if needed)
- [ ] Technical approach discussed
- [ ] Dependencies identified
- [ ] Team has asked questions

**During Estimation:**
- [ ] Everyone participates
- [ ] Outliers discussed
- [ ] Assumptions documented
- [ ] Risks identified
- [ ] Consensus reached

**After Estimation:**
- [ ] Estimate recorded
- [ ] Confidence level noted
- [ ] Story properly sized (< 13 points)
- [ ] Ready for sprint planning

---

## Tools & Resources

**Estimation Tools:**
- Planning Poker (app/cards)
- Jira estimation features
- Miro for virtual planning
- Google Sheets trackers

**Further Reading:**
- [Story Points and Estimation](https://www.atlassian.com/agile/project-management/estimation)
- [Planning Poker Guide](https://www.mountaingoatsoftware.com/agile/planning-poker)
- [User Story Splitting](https://www.humanizingwork.com/the-humanizing-work-guide-to-splitting-user-stories/)

---

## Quick Reference

### Story Point Scale
- 1 = Trivial (hours)
- 2 = Simple (1 day)
- 3 = Moderate (1-2 days)
- 5 = Average (2-3 days)
- 8 = Complex (3-5 days)
- 13 = Very complex (split it!)
- 21+ = Too large (definitely split!)

### Estimation Formula
```
Story Points = f(Complexity, Uncertainty, Effort)
```

### When to Re-estimate
- Requirements changed significantly
- Technical approach changed
- After spike reveals new information
- Story partially completed (remaining work)
