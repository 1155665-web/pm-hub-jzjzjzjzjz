# User Story Template

## Story Title
[Short, descriptive title of what the user wants to accomplish]

---

## User Story

**As a** [type of user/persona]  
**I want** [goal/desire]  
**So that** [benefit/value]

---

## Description

[Detailed explanation of the feature or functionality. Include context, background, and why this is important]

---

## Acceptance Criteria

Using the Given-When-Then format:

### Scenario 1: [Scenario name]
- **Given** [initial context/state]
- **When** [action/event occurs]
- **Then** [expected outcome]

### Scenario 2: [Scenario name]
- **Given** [initial context/state]
- **When** [action/event occurs]
- **Then** [expected outcome]

### Scenario 3: [Scenario name]
- **Given** [initial context/state]
- **When** [action/event occurs]
- **Then** [expected outcome]

---

## Additional Requirements

### Functional Requirements
- [ ] [Specific functionality requirement 1]
- [ ] [Specific functionality requirement 2]
- [ ] [Specific functionality requirement 3]

### Non-Functional Requirements
- [ ] Performance: [e.g., "Page load time < 2 seconds"]
- [ ] Security: [e.g., "Encrypt sensitive data"]
- [ ] Accessibility: [e.g., "WCAG 2.1 AA compliant"]
- [ ] Scalability: [e.g., "Handle 1000 concurrent users"]

---

## Design/Mockups

[Link to Figma/design files or attach screenshots]

---

## Technical Notes

[Any technical considerations, constraints, or implementation details that engineering should be aware of]

### API Endpoints
- [Endpoint 1]
- [Endpoint 2]

### Database Changes
- [Schema change 1]
- [Schema change 2]

### Dependencies
- [Dependency 1]
- [Dependency 2]

---

## Testing Approach

### Unit Tests
- [Test case 1]
- [Test case 2]

### Integration Tests
- [Test case 1]
- [Test case 2]

### User Acceptance Tests
- [ ] [UAT scenario 1]
- [ ] [UAT scenario 2]

---

## Edge Cases & Error Handling

- **Edge Case 1:** [Description] → [Expected behavior]
- **Edge Case 2:** [Description] → [Expected behavior]
- **Error Scenario 1:** [Description] → [Error message/handling]
- **Error Scenario 2:** [Description] → [Error message/handling]

---

## Success Metrics

**How we'll measure success:**
- [Metric 1]: [Target value]
- [Metric 2]: [Target value]
- [Metric 3]: [Target value]

**Analytics/Tracking:**
- [Event 1 to track]
- [Event 2 to track]

---

## Out of Scope

[Explicitly list what is NOT included in this story to prevent scope creep]

- [Item 1 that's out of scope]
- [Item 2 that's out of scope]

---

## Questions/Open Issues

- [ ] **Question 1:** [Question description] - [Assigned to]
- [ ] **Question 2:** [Question description] - [Assigned to]

---

## Related Stories/Epics

- [Link to Epic]
- [Link to related story 1]
- [Link to related story 2]

---

## Estimation

**Story Points:** [Points based on team's scale]

**Estimated Hours:** [If your team uses hours]

---

## Priority

- [ ] P0 - Critical (Blocker)
- [ ] P1 - High (Must have this sprint)
- [ ] P2 - Medium (Should have soon)
- [ ] P3 - Low (Nice to have)

---

## Labels/Tags

[Add relevant labels: frontend, backend, design, bug, enhancement, etc.]

---

## Example: Login Feature

**As a** new user  
**I want** to create an account with my email and password  
**So that** I can access personalized features and save my data

### Description
Users need a way to create accounts to access premium features. Currently, we only support social login, which limits our user base. This story implements traditional email/password registration.

### Acceptance Criteria

**Scenario 1: Successful Registration**
- **Given** I am on the registration page
- **When** I enter a valid email, password (8+ chars with 1 number), and accept terms
- **Then** My account is created, I receive a verification email, and I'm redirected to onboarding

**Scenario 2: Invalid Email**
- **Given** I am on the registration page
- **When** I enter an invalid email format
- **Then** I see an error "Please enter a valid email address"

**Scenario 3: Duplicate Email**
- **Given** I am on the registration page
- **When** I enter an email that's already registered
- **Then** I see "An account with this email already exists. Try logging in."

### Functional Requirements
- [ ] Email validation (valid format)
- [ ] Password must be 8+ characters with at least 1 number
- [ ] Terms and conditions checkbox required
- [ ] Verification email sent after registration
- [ ] Account created in database

### Non-Functional Requirements
- [ ] Registration completes in < 3 seconds
- [ ] Passwords hashed with bcrypt
- [ ] HTTPS only
- [ ] Rate limiting: 5 attempts per IP per hour

### Success Metrics
- Registration completion rate: > 80%
- Time to complete: < 60 seconds
- Email verification rate: > 60%

### Out of Scope
- Social login integration
- Password reset functionality (separate story)
- Profile completion
- Email preferences
