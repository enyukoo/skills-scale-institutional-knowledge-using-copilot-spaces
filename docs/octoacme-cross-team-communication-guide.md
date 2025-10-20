# OctoAcme — Cross-Team Communication Guide

## Purpose
Establish clear communication patterns and expectations for collaboration across functional teams, ensuring information flows efficiently and stakeholders stay aligned.

## Guiding Principles
- **Clarity over speed**: Take time to communicate clearly to avoid rework
- **Asynchronous first**: Respect time zones and focus time with written updates
- **Context-rich**: Provide background so recipients can make informed decisions
- **Feedback loops**: Confirm understanding and close the loop on action items
- **Transparency**: Default to open communication unless confidentiality is required

---

## Core Communication Channels

### 1. Written Updates (Async)
**Use for**: Status reports, decisions, planning docs, retrospectives

**Best Practices**:
- Use structured templates for consistency
- Include clear subject lines or titles
- Link to relevant context (issues, docs, PRs)
- Tag specific people when action is needed
- Use threading to keep conversations organized

**Recommended Tools**: GitHub Issues, Project Boards, Wiki, Email, Slack threads

### 2. Synchronous Meetings (Real-time)
**Use for**: Complex decisions, brainstorming, conflict resolution, urgent issues

**Best Practices**:
- Share agenda 24 hours in advance
- Start/end on time, respect calendars
- Document decisions and action items
- Record for those who can't attend
- Follow up with written summary

**Recommended Tools**: Video calls, standup meetings, working sessions

### 3. Direct Messages (Quick sync)
**Use for**: Quick questions, time-sensitive issues, 1:1 coordination

**Best Practices**:
- Escalate to threads or meetings if discussion grows
- Move important decisions to documented channels
- Respect "do not disturb" status
- Confirm receipt for urgent items

**Recommended Tools**: Slack, Teams, Discord DMs

---

## Team-to-Team Communication Patterns

### Developers ↔ Product Manager

**Frequency**: Weekly sync + ad-hoc as needed

**Communication Flow**:
- **Developers to PM**: Technical constraints, implementation proposals, effort estimates
- **PM to Developers**: Feature requirements, user stories, acceptance criteria, priority changes

**Key Touchpoints**:
- Sprint planning: Review backlog and clarify requirements
- Mid-sprint check-in: Validate implementation direction
- Sprint demo: Show completed work and gather feedback

**Templates to Use**:
- Feature specification template
- Technical design doc
- Estimation matrix

---

### QA Lead ↔ Developers

**Frequency**: Daily during active sprints

**Communication Flow**:
- **QA to Developers**: Test results, bug reports, reproduction steps, test coverage gaps
- **Developers to QA**: Feature readiness, test data needs, known issues, implementation details

**Key Touchpoints**:
- Daily standup: Share testing status and blockers
- PR reviews: Validate testability and edge cases
- Test planning: Define test strategy for upcoming features

**Templates to Use**:
- Bug report template (see below)
- Test plan template
- Test results summary

---

### Release Manager ↔ QA Lead

**Frequency**: Daily during release week, weekly otherwise

**Communication Flow**:
- **Release Manager to QA**: Release timeline, scope changes, deployment schedule
- **QA to Release Manager**: Test status, go/no-go recommendation, quality concerns

**Key Touchpoints**:
- Release planning: Align on testing requirements and timeline
- Pre-release sign-off: Review test results and readiness criteria
- Post-release review: Discuss quality issues and improvements

**Templates to Use**:
- Go/no-go decision template (see below)
- Release readiness checklist
- Post-release report

---

### Product Manager ↔ UX Designer

**Frequency**: 2-3x per week during design phase

**Communication Flow**:
- **PM to UX**: User problems, business requirements, success metrics, constraints
- **UX to PM**: User research findings, design concepts, usability concerns, trade-offs

**Key Touchpoints**:
- Discovery: Align on problem space and user needs
- Design reviews: Validate designs against requirements
- Implementation: Ensure design intent is preserved

**Templates to Use**:
- User story template
- Design review agenda
- Usability test findings

---

### Support Engineer ↔ Product Manager

**Frequency**: Weekly sync

**Communication Flow**:
- **Support to PM**: Customer pain points, feature requests, bug trends, usage patterns
- **PM to Support**: Roadmap updates, feature launches, known limitations, workarounds

**Key Touchpoints**:
- Weekly trends review: Discuss top customer issues
- Pre-release briefing: Share what's coming and how to support it
- Post-release follow-up: Gather customer feedback on new features

**Templates to Use**:
- Support trends report (see below)
- Release briefing for support
- Customer feedback summary

---

### Automation Specialist ↔ Developers

**Frequency**: Weekly + ad-hoc for urgent issues

**Communication Flow**:
- **Automation to Developers**: Pipeline status, tooling updates, infrastructure changes
- **Developers to Automation**: Build failures, tooling requests, performance concerns

**Key Touchpoints**:
- Sprint planning: Identify automation needs for upcoming work
- Build failures: Rapid triage and resolution
- Tooling reviews: Gather feedback on developer experience

**Templates to Use**:
- Infrastructure change notification
- Build failure report
- Tooling request form

---

## Communication Templates

### 1. Bug Report Template

```markdown
**Bug Title**: [Brief, descriptive title]

**Severity**: [Critical / High / Medium / Low]

**Environment**: [Production / Staging / Development]

**Description**:
[Clear description of the issue]

**Steps to Reproduce**:
1. [First step]
2. [Second step]
3. [Third step]

**Expected Behavior**:
[What should happen]

**Actual Behavior**:
[What actually happens]

**Screenshots/Logs**:
[Attach relevant evidence]

**Impact**:
[Who is affected and how severely]

**Workaround** (if known):
[Temporary solution]

**Related Issues**:
[Link to similar bugs or related work]
```

---

### 2. Go/No-Go Decision Template

```markdown
**Release**: [Release name/version]

**Scheduled Date**: [Deployment date and time]

**Go/No-Go Decision**: [GO / NO-GO / CONDITIONAL]

**Test Status**:
- Unit tests: [Pass/Fail] - [Coverage %]
- Integration tests: [Pass/Fail]
- End-to-end tests: [Pass/Fail]
- Performance tests: [Pass/Fail]

**Open Issues**:
- [ ] [Critical issues - count]
- [ ] [High priority issues - count]
- [ ] [Known issues accepted for release]

**Rollback Plan**: [Confirmed / Not ready]

**Stakeholder Sign-offs**:
- [ ] QA Lead: [Name] - [Approved/Declined]
- [ ] Release Manager: [Name] - [Approved/Declined]
- [ ] Product Manager: [Name] - [Approved/Declined]

**Decision Rationale**:
[Explanation of decision and any conditions]

**Next Steps**:
[What happens next based on the decision]
```

---

### 3. Support Trends Report Template

```markdown
**Reporting Period**: [Start date] to [End date]

**Executive Summary**:
[2-3 sentence overview of key trends]

**Top Issues** (by volume):
1. [Issue description] - [Ticket count]
2. [Issue description] - [Ticket count]
3. [Issue description] - [Ticket count]

**Critical Issues** (by severity):
- [Issue requiring immediate attention]
- [Customer-blocking problem]

**Feature Requests** (most requested):
1. [Feature description] - [Request count]
2. [Feature description] - [Request count]

**Customer Sentiment**:
- Satisfaction score: [Score]
- Positive feedback: [Summary]
- Areas for improvement: [Summary]

**Recommended Actions**:
- [ ] [Suggested bug fix or improvement]
- [ ] [Documentation update needed]
- [ ] [Feature consideration for roadmap]

**Attachments**:
- [Link to detailed ticket data]
- [Link to customer quotes/feedback]
```

---

## Meeting Cadence

### Daily Standups (15 min)
**Participants**: Development team, QA Lead, optional: PM, UX Designer
**Focus**: Progress, blockers, coordination

### Weekly Team Sync (30-45 min)
**Participants**: All team members
**Focus**: Progress review, risk discussion, upcoming work

### Sprint Planning (1-2 hours)
**Participants**: Developers, QA Lead, Product Manager, Project Manager, UX Designer
**Focus**: Scope next sprint, estimate work, clarify requirements

### Release Planning (1 hour)
**Participants**: Release Manager, QA Lead, Product Manager, Project Manager, Automation Specialist
**Focus**: Plan release scope, timeline, and responsibilities

### Retrospectives (45-60 min)
**Participants**: All team members
**Focus**: Review what went well, what to improve, action items

### Monthly Stakeholder Update (30 min)
**Participants**: PM, Project Manager, key stakeholders
**Focus**: Progress, roadmap, escalations

---

## Cross-Team Dependencies

### Identifying Dependencies
- Flag during planning sessions
- Document in project board or dependency tracker
- Assign clear owner for coordination
- Establish check-in cadence

### Managing Dependencies
1. **Document**: Record dependency details and impact
2. **Communicate**: Notify all affected teams early
3. **Track**: Monitor progress and escalate delays
4. **Unblock**: Work with teams to resolve blockers quickly

### Dependency Template

```markdown
**Dependent Work**: [Our task that is blocked]
**Blocking Work**: [Other team's task we need]
**Blocking Team**: [Team name]
**Contact**: [Point person on blocking team]
**Impact**: [How this affects our timeline]
**Needed By**: [Date]
**Status**: [Not started / In progress / Complete]
**Mitigation**: [Alternative if this is delayed]
```

---

## Communication Guidelines by Role

### For All Team Members
- ✅ Be responsive within 24 hours to direct questions
- ✅ Update your status regularly in shared tools
- ✅ Escalate blockers early, don't wait
- ✅ Assume positive intent in all communications
- ❌ Don't make others chase you for updates

### For Managers (PM, Project Manager)
- ✅ Provide context and priorities clearly
- ✅ Make decisions promptly to unblock teams
- ✅ Shield team from unnecessary meetings
- ✅ Communicate changes proactively
- ❌ Don't bypass individual contributors without cause

### For Cross-Functional Collaborators
- ✅ Respect each other's expertise
- ✅ Seek to understand before being understood
- ✅ Collaborate early and often
- ✅ Document shared decisions
- ❌ Don't surprise other teams with last-minute changes

---

## Escalation Paths

### Level 1: Team-Level Resolution
- **Timeline**: 1-2 days
- **Approach**: Direct communication between team members
- **Example**: Developer and QA discussing test coverage

### Level 2: Manager Resolution
- **Timeline**: 2-4 hours for urgent, 1 week for normal
- **Approach**: Project Manager or Product Manager intervenes
- **Example**: Resource conflicts or priority disputes

### Level 3: Leadership Resolution
- **Timeline**: Immediate for critical, days for strategic
- **Approach**: Director or VP makes decision
- **Example**: Major scope change or budget issue

---

## Tips for Effective Cross-Team Communication

1. **Overcommunicate early**: Especially at project start
2. **Use the right channel**: Match tool to message urgency and complexity
3. **Close the loop**: Always confirm receipt and next steps
4. **Be specific**: Vague asks lead to misalignment
5. **Document decisions**: Memory is fallible, written records aren't
6. **Build relationships**: Personal connections ease collaboration
7. **Give credit**: Acknowledge contributions publicly
8. **Learn team norms**: Respect how other teams work
9. **Feedback welcome**: Create safe space for honest input
10. **Iterate**: Improve communication based on retrospectives

---

## References
- [OctoAcme Roles and Personas](./octoacme-roles-and-personas.md)
- [OctoAcme Role Handoff Checklist](./octoacme-role-handoff-checklist.md)
- [OctoAcme Release Responsibility Matrix](./octoacme-release-responsibility-matrix.md)
- [OctoAcme Risk Management & Communication](./octoacme-risks-and-communication.md)
