# ðŸ¤– AI Developer Agent: GitHub Issues & Project Tracking Guide

Welcome to the team! To ensure our project stays organized and our progress is properly documented, you must strictly follow this workflow. We use GitHub Issues and Milestones as our single source of truth for task management and progress tracking. 

As an AI Dev Agent, you are expected to operate autonomously but with strict adherence to this documentation process.

---

## ðŸŽ¯ 1. Core Principles

- **No Code Without an Issue:** Never start writing code or making system changes without an associated GitHub Issue. 
- **Atomic Issues:** Break down large tasks into smaller, manageable issues. One issue should ideally map to one focused pull request or set of commits.
- **Always Link:** Every commit message and pull request must reference its corresponding issue number (e.g., `Fixes #12` or `Relates to #15`).
- **Milestone Alignment:** Every issue must belong to an active Milestone.
- **Continuous Updates:** Don't wait until the end of a task to update GitHub. Drop comments on the issue with your findings, blockers, and partial progress.

---

## ðŸ”„ 2. The Standard Workflow 

For every new task or chat session, follow this step-by-step process:

### Phase 1: Context & Planning
1. **Check Existing Milestones:** Query GitHub for active milestones. Know what the current sprint/goal is.
2. **Search for Existing Issues:** Before creating a new issue, check if one already exists for the task requested by the user. If it exists, read its comments for context.
3. **Create an Issue (if needed):**
   - **Title:** Clear, concise, and action-oriented (e.g., "Implement user authentication flow" instead of "login").
   - **Body:** Document the user's request, acceptance criteria, and specific details. 
   - **Labels:** Add appropriate labels (e.g., `enhancement`, `bug`, `documentation`).
   - **Assign:** Assign the issue appropriately, and pin it to the current active **Milestone**.

### Phase 2: Execution & Tracking
1. **Comment Your Plan:** Once the issue is created/identified, add a comment briefly explaining your technical approach before writing the code.
2. **Commit Often with References:** For every commit you create, include the issue number. For example: `feat: add JWT token validation (fixes #42)`
3. **Mid-task Updates:** If the task is large or complex, post a quick comment on the issue summarizing what is done so far and what remains.

### Phase 3: Review & Completion
1. **Pull Requests (or Final Commits):** 
   - Ensure the PR description links back to the issue (e.g., `Closes #12`).
   - Provide a short summary of the changes made and any verification tests performed.
2. **Close the Issue:** Only close the issue once work is verified and fully merged.
3. **Milestone Check:** After closing, review the current Milestone. If all issues in the Milestone are closed, notify the user!

---

## ðŸ› ï¸ 3. Troubleshooting & Blockers
If you run into an unexpected bug, missing dependencies, or need user feedback:
1. **Update the Issue:** Add a comment explaining the blocker.
2. **Add a Label:** If applicable, apply a label like `blocked` or `needs-review`.
3. **Notify the User:** Alert the user in the active chat that you are blocked, providing a link to the issue to explain the context.

---

## ðŸ“ 4. Example Git Commit Format
When pushing files, make sure your commit messages contain the tracking ID:

```text
[type]: [short summary] (#issue_number)

[optional detailed description]
```

**Types:** `feat`, `fix`, `docs`, `style`, `refactor`, `test`, `chore`
**Example:** `feat: implement login UI component (#12)`

### Reminder
Your job is not only to write excellent code but to maintain the structured history of this project. **Discipline is key!** Every step you take should be trackable through GitHub.
