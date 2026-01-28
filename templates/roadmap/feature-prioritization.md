# Feature Prioritization Framework

## Overview

This document provides frameworks and templates for prioritizing features and initiatives in your product backlog.

---

## Framework 1: RICE Scoring

**RICE** = (Reach × Impact × Confidence) / Effort

### How to Calculate

**Reach:** How many users will this affect per time period?
- Example: 5000 users per quarter

**Impact:** How much will this impact each user?
- 3 = Massive impact
- 2 = High impact
- 1 = Medium impact
- 0.5 = Low impact
- 0.25 = Minimal impact

**Confidence:** How sure are you about your estimates?
- 100% = High confidence
- 80% = Medium confidence
- 50% = Low confidence

**Effort:** How much time will this take?
- Measured in person-months
- Example: 2 person-months

### RICE Score Template

| Feature | Reach | Impact | Confidence | Effort | RICE Score | Priority |
|---------|-------|--------|------------|--------|------------|----------|
| [Feature 1] | 5000 | 3 | 100% | 2 | 7500 | 1 |
| [Feature 2] | 2000 | 2 | 80% | 1 | 3200 | 2 |
| [Feature 3] | 1000 | 3 | 50% | 3 | 500 | 3 |

**Example Calculation:**
```
Feature 1: Guest Checkout
- Reach: 5000 users/quarter (checkout attempts)
- Impact: 3 (massive - enables purchases)
- Confidence: 100% (well-researched)
- Effort: 2 person-months

RICE = (5000 × 3 × 1.0) / 2 = 7500
```

---

## Framework 2: Value vs Effort Matrix

Plot features on a 2x2 matrix:

```
High Value │  ⚠️ Big Bets      │  🚀 Quick Wins
           │  (High effort)    │  (Low effort)
           │                   │
───────────┼───────────────────┼──────────────
           │                   │
Low Value  │  ❌ Money Pit     │  🗑️ Maybe Later
           │  (High effort)    │  (Low effort)
           │                   │
           └───────────────────┴──────────────
              High Effort          Low Effort
```

### Feature Mapping

**Quick Wins (Do First):**
- [Feature 1]: [Brief description]
- [Feature 2]: [Brief description]

**Big Bets (Do Next if strategic):**
- [Feature 3]: [Brief description]
- [Feature 4]: [Brief description]

**Maybe Later (Fill spare capacity):**
- [Feature 5]: [Brief description]

**Money Pit (Don't do):**
- [Feature 6]: [Brief description]

---

## Framework 3: Kano Model

Categorize features by user satisfaction impact:

**Basic Needs (Must-Haves):**
- Users expect these
- Absence causes dissatisfaction
- Presence doesn't increase satisfaction
- Example: Login functionality, basic search

**Performance Needs (More is Better):**
- Linear satisfaction increase
- Better implementation = happier users
- Example: Faster page load, more accurate search

**Delighters (Wow Factor):**
- Unexpected features
- Absence doesn't cause dissatisfaction
- Presence creates delight
- Example: Easter eggs, delightful animations

**Indifferent:**
- Users don't care
- Don't prioritize these
- Example: Features you think are cool but users don't use

### Kano Template

| Feature | Category | Justification | Priority |
|---------|----------|---------------|----------|
| [Feature 1] | Basic Need | Must have for MVP | High |
| [Feature 2] | Performance | Users request faster | Medium |
| [Feature 3] | Delighter | Competitive advantage | Low |
| [Feature 4] | Indifferent | No user demand | None |

---

## Framework 4: MoSCoW Method

**M**ust have  
**S**hould have  
**C**ould have  
**W**on't have (this time)

### MoSCoW Template

**Must Have (Critical):**
- [ ] [Feature 1]: [Why critical]
- [ ] [Feature 2]: [Why critical]
- [ ] [Feature 3]: [Why critical]

**Should Have (Important but not critical):**
- [ ] [Feature 4]: [Why important]
- [ ] [Feature 5]: [Why important]

**Could Have (Nice to have):**
- [ ] [Feature 6]: [Why nice to have]
- [ ] [Feature 7]: [Why nice to have]

**Won't Have (Not this release):**
- [ ] [Feature 8]: [Why not now]
- [ ] [Feature 9]: [Why not now]

---

## Framework 5: Weighted Scoring

Define criteria important to your product, assign weights, score each feature.

### Weighted Scoring Template

**Criteria & Weights:**
- User Value: 30%
- Business Value: 25%
- Effort (inverse): 20%
- Strategic Alignment: 15%
- Risk (inverse): 10%

| Feature | User Value (30%) | Business Value (25%) | Effort (20%) | Strategy (15%) | Risk (10%) | Total Score |
|---------|------------------|----------------------|--------------|----------------|------------|-------------|
| [Feature 1] | 9 | 8 | 7 | 9 | 8 | 8.35 |
| [Feature 2] | 7 | 9 | 9 | 7 | 7 | 7.85 |
| [Feature 3] | 8 | 6 | 5 | 8 | 9 | 7.15 |

**Scoring Scale:** 1-10 (10 = best)

**Example Calculation for Feature 1:**
```
Total = (9×0.30) + (8×0.25) + (7×0.20) + (9×0.15) + (8×0.10)
      = 2.7 + 2.0 + 1.4 + 1.35 + 0.8
      = 8.35
```

---

## Framework 6: ICE Score

**ICE** = Impact × Confidence × Ease

Simpler than RICE, good for quick prioritization.

### ICE Scoring Template

| Feature | Impact (1-10) | Confidence (1-10) | Ease (1-10) | ICE Score | Priority |
|---------|---------------|-------------------|-------------|-----------|----------|
| [Feature 1] | 9 | 8 | 7 | 504 | 1 |
| [Feature 2] | 8 | 7 | 6 | 336 | 2 |
| [Feature 3] | 7 | 9 | 8 | 504 | 1 |

**Example:**
```
Feature: One-Click Checkout
- Impact: 9 (will significantly increase conversions)
- Confidence: 8 (have data supporting this)
- Ease: 7 (moderate implementation effort)

ICE = 9 × 8 × 7 = 504
```

---

## Framework 7: Opportunity Scoring

Survey users on two dimensions:
1. How important is this? (1-10)
2. How satisfied are you? (1-10)

**Opportunity Score** = Importance + (Importance - Satisfaction)

### Opportunity Template

| Feature | Importance | Satisfaction | Opportunity Score | Priority |
|---------|------------|--------------|-------------------|----------|
| [Feature 1] | 9 | 3 | 15 | High |
| [Feature 2] | 7 | 6 | 8 | Medium |
| [Feature 3] | 8 | 8 | 8 | Medium |

**Highest opportunity** = Important but users are unsatisfied

**Example:**
```
Feature: Search functionality
- Importance: 9 (users say it's critical)
- Satisfaction: 3 (users very unhappy with current)

Opportunity = 9 + (9 - 3) = 15 (High priority!)
```

---

## Comprehensive Prioritization Template

Use this for thorough analysis of major features:

### Feature: [Feature Name]

**Description:**
[Brief description of the feature]

---

#### 1. Business Case

**Problem:**
[What problem does this solve?]

**Solution:**
[How does this feature solve it?]

**Target Users:**
[Who is this for?]

---

#### 2. Value Assessment

**User Value:**
- [Benefit 1]
- [Benefit 2]
- [Benefit 3]

**Business Value:**
- Revenue impact: [Estimate]
- Cost savings: [Estimate]
- Strategic importance: [Rating 1-10]

---

#### 3. Effort Estimation

**Development Effort:**
- Story points: [X]
- Time estimate: [Y] sprints / [Z] weeks
- Team: [Which team(s)]

**Complexity:**
- Technical: [Low/Medium/High]
- Design: [Low/Medium/High]
- Testing: [Low/Medium/High]

---

#### 4. Risk Assessment

**Technical Risks:**
- [Risk 1]: [Impact] - [Mitigation]

**Business Risks:**
- [Risk 1]: [Impact] - [Mitigation]

**Overall Risk:** [Low/Medium/High]

---

#### 5. Data & Evidence

**User Research:**
- [Finding 1]
- [Finding 2]

**Analytics:**
- [Data point 1]
- [Data point 2]

**Customer Requests:**
- [X] customers requested this
- [Y]% of support tickets relate to this

---

#### 6. Dependencies

**Prerequisites:**
- [Dependency 1]
- [Dependency 2]

**Blockers:**
- [Blocker 1]
- [Blocker 2]

---

#### 7. Success Metrics

**How we'll measure success:**
- [Metric 1]: [Target]
- [Metric 2]: [Target]
- [Metric 3]: [Target]

---

#### 8. Scoring Summary

| Framework | Score | Ranking |
|-----------|-------|---------|
| RICE | [X] | [Rank] |
| ICE | [Y] | [Rank] |
| Value/Effort | [Quadrant] | [Rank] |
| MoSCoW | [Category] | - |

**Recommended Priority:** [High/Medium/Low]

---

## Quick Decision Matrix

When you need to prioritize quickly, use this simplified approach:

| Feature | Must Do? | Easy Win? | Strategic? | Customer Demand? | Decision |
|---------|----------|-----------|------------|------------------|----------|
| [F1] | ✅ | ✅ | ✅ | ✅ | **Do Now** |
| [F2] | ❌ | ✅ | ✅ | ❌ | Do Next |
| [F3] | ❌ | ❌ | ✅ | ✅ | Do Later |
| [F4] | ❌ | ❌ | ❌ | ❌ | Don't Do |

---

## Prioritization Meeting Agenda

**Duration:** 2 hours  
**Attendees:** PM, Engineering Lead, Design Lead, Key Stakeholders

### Agenda

1. **Context (10 min)**
   - Business goals
   - User needs
   - Technical constraints

2. **Feature Review (60 min)**
   - Present each feature
   - Discuss value and effort
   - Clarify assumptions

3. **Scoring (30 min)**
   - Apply chosen framework
   - Discuss scores
   - Reach consensus

4. **Prioritization (15 min)**
   - Rank features
   - Identify must-haves
   - Set timeline

5. **Next Steps (5 min)**
   - Document decisions
   - Assign owners
   - Schedule follow-up

---

## Tips for Effective Prioritization

**DO:**
✅ Use data to inform decisions  
✅ Consider multiple frameworks  
✅ Include diverse perspectives  
✅ Re-prioritize regularly  
✅ Be transparent about criteria  
✅ Document reasoning  
✅ Say no to low-value work  

**DON'T:**
❌ Prioritize based on who shouts loudest  
❌ Ignore effort considerations  
❌ Commit to everything  
❌ Forget about technical debt  
❌ Neglect strategic initiatives  
❌ Change priorities too frequently  
❌ Prioritize without criteria  

---

## Common Prioritization Challenges

**Challenge:** Everything is high priority
**Solution:** Force rank, use MoSCoW, limit "must haves"

**Challenge:** Stakeholders disagree
**Solution:** Use data, apply consistent framework, escalate if needed

**Challenge:** Technical debt vs features
**Solution:** Allocate 20% capacity to debt, show business impact

**Challenge:** Urgent vs important
**Solution:** Have buffer for urgent, protect time for important

**Challenge:** Long-term vs short-term
**Solution:** Balance quick wins with strategic bets (70/20/10 rule)

---

## Resources

- [RICE Prioritization](https://www.intercom.com/blog/rice-simple-prioritization-for-product-managers/)
- [Kano Model](https://www.mindtheproduct.com/kano-model/)
- [Opportunity Scoring](https://strategyn.com/customer-centered-innovation-map/)
- [Weighted Scoring Model](https://www.productplan.com/glossary/weighted-scoring/)
