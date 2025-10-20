# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## Release Manager

### Role Summary
Release Managers coordinate and execute software releases, ensuring deployments are safe, timely, and well-communicated. They bridge development, operations, and stakeholder communications during the release lifecycle.

### Responsibilities
- Plan and schedule release windows and deployment activities
- Coordinate go/no-go decisions with PM, QA, and engineering
- Maintain release notes and changelogs
- Execute deployment checklists and monitor rollouts
- Manage rollback procedures if issues arise
- Communicate release status to stakeholders and support teams

### Goals
- Ensure zero-downtime deployments when possible
- Minimize production incidents related to releases
- Maintain clear audit trail of what was deployed when

### Typical Communication
- Pre-release planning meetings with PM and engineering leads
- Release announcements to stakeholders and support
- Post-deployment status updates and retrospectives
- Coordination with on-call teams during deployment windows

### Interactions with Other Roles
- **Developers**: Receive builds and coordinate merge/release timing
- **QA Lead**: Validate release readiness and sign-off
- **Project Manager**: Align release schedules with project milestones
- **Support Engineer**: Provide release notes and known issues
- **Automation Specialist**: Collaborate on CI/CD pipeline improvements

---

## QA Lead

### Role Summary
QA Leads ensure product quality by defining testing strategies, coordinating test execution, and validating that acceptance criteria are met before releases.

### Responsibilities
- Define test strategy and approach for projects
- Coordinate test execution across unit, integration, and end-to-end tests
- Review and validate acceptance criteria with Product Managers
- Identify quality gaps and advocate for fixes before release
- Maintain test documentation and test data management
- Report on quality metrics and test coverage

### Goals
- Prevent defects from reaching production
- Ensure comprehensive test coverage for critical paths
- Advocate for testability in feature design

### Typical Communication
- Daily coordination with developers on test results
- Sprint planning input on testing requirements
- Pre-release sign-off meetings with Release Manager
- Quality metrics reporting to Project Manager

### Interactions with Other Roles
- **Developers**: Collaborate on test case design and bug triage
- **Product Manager**: Validate acceptance criteria and edge cases
- **Release Manager**: Provide go/no-go recommendation for releases
- **UX Designer**: Test usability and user flows
- **Automation Specialist**: Define automation priorities and review test frameworks

---

## UX Designer

### Role Summary
UX Designers create user-centered designs that balance business goals with user needs. They conduct research, create prototypes, and collaborate with engineering to deliver intuitive experiences.

### Responsibilities
- Conduct user research and usability testing
- Create wireframes, mockups, and interactive prototypes
- Define user flows and interaction patterns
- Maintain design system consistency
- Collaborate with developers on implementation feasibility
- Validate final implementations against design specs

### Goals
- Deliver intuitive, accessible user experiences
- Reduce user friction and increase satisfaction
- Ensure design consistency across products

### Typical Communication
- Design reviews with Product Managers and stakeholders
- Collaboration sessions with developers during implementation
- User research readouts and usability findings
- Design system updates and component specifications

### Interactions with Other Roles
- **Product Manager**: Align designs with product requirements and user stories
- **Developers**: Collaborate on implementation and feasibility
- **QA Lead**: Define expected user flows for testing
- **Support Engineer**: Gather feedback on user pain points

---

## Support Engineer

### Role Summary
Support Engineers serve as the frontline for customer issues, troubleshooting problems, documenting patterns, and feeding insights back to product and engineering teams.

### Responsibilities
- Respond to customer support tickets and inquiries
- Troubleshoot and diagnose technical issues
- Document known issues and workarounds
- Escalate bugs and feature requests to engineering
- Maintain support documentation and FAQs
- Track support metrics and identify recurring issues

### Goals
- Provide timely, helpful responses to customers
- Reduce mean time to resolution (MTTR)
- Surface product improvements based on customer feedback

### Typical Communication
- Daily ticket triage and escalations
- Weekly sync with Product Manager on customer trends
- Release briefings from Release Manager on new features
- Bug reports and feedback to developers

### Interactions with Other Roles
- **Product Manager**: Report customer needs and pain points
- **Developers**: Escalate bugs and provide reproduction steps
- **Release Manager**: Receive release notes and known issues
- **QA Lead**: Report edge cases found in production
- **UX Designer**: Share user feedback on confusing interfaces

---

## Automation Specialist

### Role Summary
Automation Specialists build and maintain CI/CD pipelines, test automation frameworks, and infrastructure-as-code to improve development velocity and reliability.

### Responsibilities
- Design and maintain CI/CD pipelines
- Build and optimize test automation frameworks
- Implement infrastructure-as-code and deployment automation
- Monitor build and deployment health
- Provide tooling and training to improve team productivity
- Identify opportunities for process automation

### Goals
- Minimize manual, repetitive work through automation
- Reduce build and deployment cycle times
- Improve test reliability and coverage

### Typical Communication
- Infrastructure and tooling updates in team standups
- Pipeline troubleshooting with developers
- Automation roadmap reviews with Project Manager
- Post-deployment reviews with Release Manager

### Interactions with Other Roles
- **Developers**: Enable efficient workflows through tooling
- **QA Lead**: Build test automation frameworks and infrastructure
- **Release Manager**: Automate deployment processes
- **Project Manager**: Report on automation ROI and velocity improvements

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

