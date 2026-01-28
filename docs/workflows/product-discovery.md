# Product Discovery Process

## Overview

Product discovery is the continuous process of understanding customer problems, validating solutions, and determining what to build. It happens before and alongside product delivery.

## Discovery vs. Delivery

| Discovery | Delivery |
|-----------|----------|
| What should we build? | How do we build it? |
| Is this the right problem? | Is this built correctly? |
| Will customers use this? | Does it meet requirements? |
| Fast, cheap experiments | Production-quality code |
| Learning and validation | Shipping and monitoring |

## The Discovery Process

```
Problem Identification → Research → Ideation → Validation → Prioritization
         ↑                                                         ↓
         └──────────────────── Continuous Loop ──────────────────┘
```

---

## Phase 1: Problem Identification

### Sources of Problems

**Customer Feedback:**
- Support tickets
- User interviews
- Surveys
- Feature requests
- Usage data

**Business Needs:**
- Company goals
- Market opportunities
- Competitive threats
- Revenue targets

**Technical Factors:**
- Technical debt
- Performance issues
- Scalability limits
- Security concerns

**Team Insights:**
- Developer observations
- Design feedback
- Sales input
- Customer success insights

### Problem Statement Template

```markdown
## Problem Statement

**Who:** [Target user/customer segment]

**What:** [The problem they're experiencing]

**Where:** [Context/situation where problem occurs]

**When:** [Frequency/timing of the problem]

**Why it matters:** [Business/user impact]

**Current workaround:** [How users solve it today]

**Success criteria:** [How we'll know it's solved]
```

### Example Problem Statement

```markdown
## User Authentication Problem

**Who:** New users trying to sign up for our platform

**What:** Complex password requirements causing sign-up abandonment

**Where:** Registration page, during account creation

**When:** Happening to ~30% of sign-up attempts

**Why it matters:** 
- Losing potential customers
- ~$50K MRR impact
- Poor first impression

**Current workaround:** 
- Users contact support for help
- Some give up entirely

**Success criteria:** 
- Reduce sign-up abandonment by 50%
- Decrease support tickets by 30%
- Increase new user activation
```

---

## Phase 2: User Research

### Research Methods

**Qualitative Research:**

1. **User Interviews**
   - One-on-one conversations
   - 30-60 minutes each
   - 5-8 interviews per segment
   - Open-ended questions
   
2. **Contextual Inquiry**
   - Observe users in their environment
   - See actual workflows
   - Uncover unstated needs
   
3. **Diary Studies**
   - Users log experiences over time
   - Capture patterns and contexts
   - Good for infrequent behaviors

**Quantitative Research:**

1. **Surveys**
   - Large sample size
   - Statistical significance
   - Multiple choice + some open-ended
   
2. **Analytics**
   - Usage patterns
   - Feature adoption
   - Funnel analysis
   - Cohort analysis
   
3. **A/B Tests**
   - Compare variations
   - Measure behavior, not opinions
   - Statistical rigor required

### Interview Guide Template

```markdown
## Interview Guide: [Topic]

**Goal:** [What you want to learn]

**Participants:** [Target user type]

**Duration:** 45 minutes

### Introduction (5 min)
- Thank them for their time
- Explain purpose
- Get consent to record
- Assure confidentiality

### Warm-up (5 min)
- Tell me about your role
- How long have you been doing this?
- What's a typical day like?

### Current State (15 min)
- Walk me through how you [do task X]
- What tools do you use?
- What works well?
- What's frustrating?

### Problem Deep-Dive (15 min)
- Tell me about a time when [problem occurred]
- How did you handle it?
- What would have made it easier?
- How often does this happen?

### Wrap-up (5 min)
- If you could wave a magic wand, what would you change?
- Is there anything else you'd like to share?
- Can we follow up if we have more questions?
```

### Research Analysis

**Affinity Mapping:**
1. Write each insight on a sticky note
2. Group similar insights together
3. Label each group
4. Look for patterns across groups
5. Identify key themes

**Common Themes:**
- Pain points
- Desired outcomes
- Workarounds
- Jobs to be done
- Unmet needs

---

## Phase 3: Ideation

### Brainstorming Sessions

**Preparation:**
- Define the problem clearly
- Share background research
- Set time limit (45-60 min)
- Prepare space (physical or virtual board)

**Rules:**
1. Quantity over quality
2. No criticism
3. Build on others' ideas
4. Encourage wild ideas
5. Stay focused on problem

**Techniques:**

**Crazy 8s:**
- Fold paper into 8 sections
- 5 minutes total
- Sketch one idea per section
- Forces rapid ideation

**How Might We:**
- Rephrase problems as questions
- "How might we make password creation easier?"
- Generates solution-focused thinking

**Reverse Brainstorming:**
- "How might we make this problem worse?"
- Then reverse those ideas
- Uncovers non-obvious solutions

### Solution Sketching

**Low-Fidelity Sketches:**
- Paper and pencil
- Quick and rough
- Focus on concepts, not details
- Easy to iterate and discard

**Key Elements:**
- User flow
- Main interactions
- Core functionality
- Value proposition

---

## Phase 4: Validation

### Validation Methods

**1. Prototype Testing**

**Paper Prototypes:**
- Drawings of interface
- Very low cost
- Fast to create and iterate
- Good for early concepts

**Clickable Prototypes:**
- Figma, InVision, etc.
- More realistic
- Can test flows
- Good for validation

**Testing Process:**
1. Create prototype
2. Write test scenarios
3. Recruit 5-8 users
4. Observe them using prototype
5. Ask follow-up questions
6. Iterate based on feedback

**2. Concierge MVP**

- Manually provide the service
- Validates demand before building
- Learn what features matter most
- Example: Manually send curated content before building algorithm

**3. Wizard of Oz**

- Appears automated but is manual
- Frontend seems to work
- Backend is human-powered
- Tests concept without full build

**4. Landing Page Test**

- Create marketing page
- Drive traffic
- Measure sign-ups
- Validates demand

**5. Fake Door Test**

- Add UI for feature that doesn't exist
- Track click rate
- Shows interest level
- Explain feature isn't ready yet to those who click

### Success Criteria

Define upfront what success looks like:

**Qualitative:**
- "Users can complete task without help"
- "Users express excitement about solution"
- "Solution addresses stated pain point"

**Quantitative:**
- "80% task completion rate"
- "Less than 5 seconds to complete action"
- "10% click-through rate on landing page"

---

## Phase 5: Prioritization

### Prioritization Frameworks

**1. RICE Score**

```
RICE = (Reach × Impact × Confidence) / Effort
```

- **Reach:** Users affected per time period
- **Impact:** Scale of 3 (massive) to 0.25 (minimal)
- **Confidence:** Percentage (100% = high, 50% = low)
- **Effort:** Person-months

**Example:**
```
Feature A:
Reach: 5000 users/quarter
Impact: 2 (high)
Confidence: 80%
Effort: 2 person-months

RICE = (5000 × 2 × 0.8) / 2 = 4000
```

**2. Value vs. Effort Matrix**

```
High Value  │  ⚠️  Quick Wins │  🚀  Big Bets
Low Effort  │               │  High Effort
─────────────┼───────────────┼─────────────
Low Value   │  🗑️  Low Priority │  ❌  Money Pit
Low Effort  │               │  High Effort
```

**3. MoSCoW Method**

- **Must Have:** Non-negotiable, critical
- **Should Have:** Important but not critical
- **Could Have:** Nice to have
- **Won't Have:** Explicitly out of scope

**4. Kano Model**

- **Basic Needs:** Must have, users expect it
- **Performance Needs:** More is better
- **Delighters:** Unexpected, create wow factor

### Opportunity Scoring

Survey users on two dimensions:
1. How important is this? (1-10)
2. How satisfied are you with current solution? (1-10)

**Opportunity = Importance + (Importance - Satisfaction)**

High opportunity = Important AND dissatisfied

---

## Discovery Cadence

### Continuous Discovery

**Weekly:**
- Review customer feedback
- Analyze usage data
- Brief user interviews (2-3)

**Bi-weekly:**
- Team discovery sessions
- Share research findings
- Prioritize problems

**Monthly:**
- Deep-dive research on key topics
- Competitive analysis
- Trend analysis

**Quarterly:**
- Major user research initiatives
- Market research
- Strategic planning

---

## Discovery Outputs

### Key Deliverables

**1. Opportunity Solution Tree**
- Desired outcome at top
- Opportunities (problems) below
- Solutions for each opportunity
- Experiments to test solutions

**2. Assumption Mapping**
- List all assumptions
- Plot on: Important vs. Evidence
- Test high-importance, low-evidence assumptions first

**3. Customer Journey Map**
- Stages of customer interaction
- Actions at each stage
- Pain points
- Opportunities

**4. Job Story**
- "When [situation], I want to [motivation], so I can [expected outcome]"
- More context than user stories
- Focus on circumstances, not personas

**5. Product Brief**
- Problem statement
- Research summary
- Proposed solution
- Success metrics
- Risks and mitigations

---

## Discovery Tools

### Research Tools
- **UserTesting:** Remote user testing
- **Maze:** Rapid prototyping testing
- **Hotjar:** Heatmaps and recordings
- **Dovetail:** Research repository

### Analysis Tools
- **Miro:** Collaborative whiteboarding
- **FigJam:** Brainstorming and mapping
- **Airtable:** Tracking and organizing research
- **Notion:** Documentation and knowledge base

### Prototyping Tools
- **Figma:** High-fidelity prototypes
- **Balsamiq:** Low-fidelity wireframes
- **InVision:** Clickable prototypes
- **Marvel:** Quick mobile prototypes

---

## Discovery Anti-Patterns

### What Not to Do

**❌ Building without validation**
- Assumption: "I know what users want"
- Risk: Build something no one needs

**❌ Only listening to loud users**
- Assumption: "Squeaky wheel = most important"
- Risk: Optimize for minority, ignore silent majority

**❌ Analysis paralysis**
- Assumption: "Need more data before deciding"
- Risk: Never ship, miss opportunities

**❌ Confirmation bias**
- Assumption: "My idea is right"
- Risk: Ignore contradictory evidence

**❌ HiPPO (Highest Paid Person's Opinion)**
- Assumption: "Boss knows best"
- Risk: Build for internal politics, not users

**✅ Good Discovery Habits**

- Talk to users continuously
- Test assumptions early
- Embrace being wrong
- Iterate based on evidence
- Ship small, learn fast

---

## Discovery Checklist

Before moving to delivery:

- [ ] Problem is clearly defined
- [ ] Talked to at least 5 target users
- [ ] Validated problem exists and matters
- [ ] Explored multiple solutions
- [ ] Tested preferred solution with users
- [ ] Defined success metrics
- [ ] Confirmed technical feasibility
- [ ] Prioritized against other opportunities
- [ ] Stakeholders aligned
- [ ] Team understands the why

---

## Resources

- [Continuous Discovery Habits](https://www.producttalk.org/2021/05/continuous-discovery-habits/) by Teresa Torres
- [The Mom Test](http://momtestbook.com/) by Rob Fitzpatrick
- [Sprint](https://www.thesprintbook.com/) by Jake Knapp
- [Lean Customer Development](https://www.cindyalvarez.com/lean-customer-development) by Cindy Alvarez
