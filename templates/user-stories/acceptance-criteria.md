# Acceptance Criteria Template

## What are Acceptance Criteria?

Acceptance criteria are the conditions that a feature or user story must satisfy to be accepted by the product owner and considered "done." They define the boundaries of a story and help the team understand what needs to be built.

---

## Best Practices

### DO:
✅ Write criteria before development starts  
✅ Make them specific and testable  
✅ Focus on the "what," not the "how"  
✅ Include both happy path and edge cases  
✅ Keep them clear and concise  
✅ Review with the team  

### DON'T:
❌ Be vague or ambiguous  
❌ Include implementation details  
❌ Write too many (keep it focused)  
❌ Skip error scenarios  
❌ Make them too technical  

---

## Format 1: Given-When-Then (Recommended)

Most clear and structured format:

```
Given [precondition/context]
When [action/event]
Then [expected outcome]
```

### Example: Search Functionality

**Scenario 1: Successful search**
- **Given** I am on the home page
- **When** I enter "laptop" in the search box and click Search
- **Then** I see a list of products containing "laptop" in their name or description

**Scenario 2: No results**
- **Given** I am on the home page
- **When** I search for "xyznonexistentitem"
- **Then** I see a message "No results found for 'xyznonexistentitem'" and suggestions for popular items

**Scenario 3: Empty search**
- **Given** I am on the home page
- **When** I click Search without entering any text
- **Then** I see an error message "Please enter a search term"

---

## Format 2: Checklist Format

Simple and quick:

```
- [ ] Criterion 1
- [ ] Criterion 2
- [ ] Criterion 3
```

### Example: User Profile Update

- [ ] User can update their first name
- [ ] User can update their last name
- [ ] User can update their phone number
- [ ] User can upload a profile picture (max 5MB, jpg/png only)
- [ ] Changes are saved when clicking "Save Changes" button
- [ ] User sees confirmation message "Profile updated successfully"
- [ ] Changes are reflected immediately in the UI
- [ ] If upload fails, user sees specific error message
- [ ] Form validates phone number format
- [ ] Required fields show error if left empty

---

## Format 3: Scenario-Based

Organized by user flows:

### Example: Checkout Process

**Main Flow:**
1. User reviews items in cart
2. User enters shipping address
3. User selects shipping method
4. User enters payment information
5. User reviews order summary
6. User confirms order
7. User sees order confirmation with order number

**Alternative Flows:**
- **Guest Checkout:** User can checkout without creating account
- **Saved Address:** Returning users see their saved addresses
- **Promo Code:** User can apply discount code at checkout

**Error Flows:**
- **Invalid Card:** Show "Payment declined. Please use a different card."
- **Out of Stock:** Show which items are unavailable, allow removing them
- **Network Error:** Show retry option with "Connection lost. Please try again."

---

## Common Patterns

### User Input Validation

```
- [ ] Accepts valid input format
- [ ] Rejects invalid input format with specific error message
- [ ] Handles empty input appropriately
- [ ] Shows real-time validation feedback
- [ ] Validates on blur and on submit
- [ ] Error messages are clear and actionable
```

### CRUD Operations (Create, Read, Update, Delete)

**Create:**
- [ ] Required fields are validated
- [ ] Success confirmation shown
- [ ] New item appears in list
- [ ] Form clears after successful creation

**Read:**
- [ ] All relevant data displayed
- [ ] Data is formatted correctly
- [ ] Handles loading state
- [ ] Handles no data state

**Update:**
- [ ] Changes are saved
- [ ] Optimistic UI update
- [ ] Confirmation message shown
- [ ] Can cancel changes

**Delete:**
- [ ] Confirmation dialog appears
- [ ] Item removed from list after confirmation
- [ ] Undo option available (if appropriate)
- [ ] Cannot delete if dependencies exist

### Error Handling

```
- [ ] Clear error message shown to user
- [ ] Error doesn't break the UI
- [ ] User can retry the action
- [ ] Error is logged for debugging
- [ ] Graceful degradation when service unavailable
```

### Performance

```
- [ ] Page loads in < 3 seconds on 4G connection
- [ ] Handles 1000+ items without lag
- [ ] Shows loading indicator for operations > 1 second
- [ ] Infinite scroll loads next page smoothly
```

### Accessibility

```
- [ ] Keyboard navigable (Tab, Enter, Esc work)
- [ ] Screen reader compatible
- [ ] Color contrast meets WCAG AA standards
- [ ] Focus indicators visible
- [ ] Alt text for all images
```

### Security

```
- [ ] User input sanitized to prevent XSS
- [ ] Authentication required for protected actions
- [ ] Authorization checked (user can only edit own data)
- [ ] Sensitive data encrypted in transit and at rest
- [ ] Rate limiting prevents abuse
```

---

## Edge Cases to Consider

### Data Scenarios
- Empty state (no data)
- Single item
- Maximum items (pagination/limits)
- Duplicate entries
- Special characters in text
- Very long text/names
- International characters (unicode)

### User Scenarios
- First-time user
- Returning user
- Anonymous user
- Admin user
- Concurrent users editing same data

### Technical Scenarios
- Slow network
- No network connection
- API timeout
- Server error
- Browser compatibility
- Mobile vs. desktop

---

## Real-World Examples

### Example 1: Password Reset

**Given** I am on the login page  
**When** I click "Forgot Password?"  
**Then** I am taken to the password reset page

**Given** I am on the password reset page  
**When** I enter my registered email and click "Send Reset Link"  
**Then** I see "If an account exists with this email, you'll receive a reset link"

**Given** I received the reset email  
**When** I click the reset link (valid for 24 hours)  
**Then** I am taken to a page to create a new password

**Given** I am creating a new password  
**When** I enter a password that meets requirements (8+ chars, 1 number, 1 special char)  
**Then** My password is updated and I'm redirected to login

**Edge Cases:**
- [ ] Link expires after 24 hours with clear error message
- [ ] Can't reuse last 3 passwords
- [ ] Email not found: same message as success (security)
- [ ] Password requirements shown and validated in real-time

---

### Example 2: File Upload

**Functional Criteria:**
- [ ] User can select files via file picker
- [ ] User can drag and drop files
- [ ] Accepts .pdf, .doc, .docx files only
- [ ] Maximum file size: 10MB
- [ ] Shows upload progress bar
- [ ] Shows file name and size after upload
- [ ] User can remove uploaded file before submitting
- [ ] Multiple files can be uploaded (up to 5)

**Error Handling:**
- [ ] Invalid file type: "Only PDF and Word documents are supported"
- [ ] File too large: "File must be under 10MB. Your file is X MB."
- [ ] Upload fails: "Upload failed. Please try again."
- [ ] Network interruption: Retry automatically up to 3 times

**Success:**
- [ ] Success message: "File uploaded successfully"
- [ ] File appears in list with correct icon
- [ ] Can download file after upload to verify

---

### Example 3: Notifications

**Given** I am logged in  
**When** Someone mentions me in a comment  
**Then** I receive an in-app notification and an email notification

**Criteria:**
- [ ] Notification appears in notification center
- [ ] Notification count badge updates
- [ ] Clicking notification takes me to relevant content
- [ ] Notification is marked as read when viewed
- [ ] Can mark all as read
- [ ] Email notification sent within 5 minutes
- [ ] Email includes link to content
- [ ] Can unsubscribe from email notifications
- [ ] Notifications load quickly (< 1 second)
- [ ] Shows most recent 50 notifications

---

## Testing Acceptance Criteria

Each acceptance criterion should be:

**Testable:** Can you write a test for it?  
**Clear:** Does everyone understand what it means?  
**Achievable:** Can it be implemented in this sprint?  
**Independent:** Not dependent on other unclear stories?  
**Valuable:** Does it add value for the user?  

---

## Acceptance Criteria Checklist

Before marking a story as "ready":

- [ ] All criteria are specific and measurable
- [ ] Happy path is covered
- [ ] Error scenarios are included
- [ ] Edge cases are addressed
- [ ] Acceptance criteria match the story description
- [ ] Team understands and agrees with criteria
- [ ] Criteria are testable
- [ ] Non-functional requirements included (if applicable)
- [ ] No ambiguous terms (e.g., "fast," "easy," "nice")

---

## Resources

- [Writing Acceptance Criteria](https://www.mountaingoatsoftware.com/blog/writing-good-user-stories)
- [Given-When-Then Format](https://cucumber.io/docs/gherkin/reference/)
- [Acceptance Test-Driven Development](https://en.wikipedia.org/wiki/Acceptance_test%E2%80%93driven_development)
