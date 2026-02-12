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

## Quality Assurance Lead

### Role Summary
Quality Assurance Leads ensure project deliverables meet agreed quality standards and acceptance criteria. They work closely with developers and product owners to verify functionality, manage defect triage, and maintain testing documentation.

### Responsibilities
- Define and maintain quality standards and testing strategies
- Verify deliverables meet acceptance criteria and quality gates
- Manage defect triage, prioritization, and resolution tracking
- Conduct acceptance testing and user acceptance test (UAT) coordination
- Maintain test documentation and quality metrics
- Collaborate with developers on test automation and quality practices

### Goals
- Ensure high-quality deliverables that meet customer expectations
- Reduce defect escape rate to production
- Maintain comprehensive test coverage and documentation
- Enable fast, confident releases through automated testing

### Typical Communication
- Daily standup participation and defect reviews
- Weekly quality reports and metrics dashboards
- Test plan reviews with Product Managers
- Defect triage meetings with developers

### Interactions with Other Roles
- **Developers**: Reviews code quality, provides feedback on testability, collaborates on fixing defects
- **Product Managers**: Validates acceptance criteria, participates in backlog refinement, confirms feature completeness
- **Project Managers**: Reports on quality metrics, identifies quality risks, provides release readiness input
- **Deployment Coordinator**: Collaborates on release testing and smoke test execution

---

## Business Analyst

### Role Summary
Business Analysts bridge the gap between business stakeholders and technical teams. They gather requirements, analyze stakeholder needs, document processes, and ensure clear communication between business and technical domains.

### Responsibilities
- Elicit and document business requirements from stakeholders
- Analyze and model business processes and workflows
- Create functional specifications and user stories
- Facilitate requirements workshops and validation sessions
- Maintain requirements traceability and documentation
- Support UAT planning and stakeholder training

### Goals
- Ensure technical solutions align with business needs
- Reduce requirement ambiguity and rework
- Enable effective communication across business and technical teams
- Improve requirement quality and completeness

### Typical Communication
- Requirements workshops with stakeholders
- Backlog refinement sessions with Product Managers and developers
- Weekly requirement reviews and documentation updates
- UAT coordination with QA Lead and stakeholders

### Interactions with Other Roles
- **Product Managers**: Collaborates on requirement definition, helps prioritize backlog, validates business value
- **Developers**: Clarifies requirements, answers technical questions, validates implementation approach
- **QA Lead**: Defines acceptance criteria, supports test case creation, validates test coverage
- **External Stakeholders**: Gathers requirements, validates solutions, facilitates feedback sessions

---

## Change Manager

### Role Summary
Change Managers oversee change control processes, ensuring all changes are properly evaluated, approved, and documented. They coordinate impact analysis, manage change approval workflows, and maintain change documentation.

### Responsibilities
- Manage change request intake and evaluation
- Coordinate impact analysis across affected teams
- Facilitate change advisory board (CAB) meetings
- Track change approvals and ensure proper authorization
- Maintain change documentation and audit trails
- Monitor change success rates and post-implementation reviews

### Goals
- Minimize disruption from changes to systems and processes
- Ensure changes are properly evaluated and authorized
- Maintain compliance with change management policies
- Enable fast, safe changes through streamlined processes

### Typical Communication
- Weekly CAB meetings for change review and approval
- Change request documentation and impact assessments
- Post-implementation review reports
- Escalation communications for emergency changes

### Interactions with Other Roles
- **Project Managers**: Coordinates project-related changes, aligns on timeline impacts, manages dependencies
- **Deployment Coordinator**: Reviews deployment plans, validates change windows, coordinates release schedules
- **Developers**: Evaluates technical change requests, assesses implementation risks
- **External Stakeholders**: Communicates change impacts, manages expectations, gathers feedback

---

## Deployment Coordinator

### Role Summary
Deployment Coordinators plan and execute release activities, ensuring smooth deployments to production. They manage deployment schedules, coordinate with operations teams, and verify release readiness.

### Responsibilities
- Plan deployment schedules and coordinate release windows
- Verify pre-deployment readiness checks are complete
- Execute deployment runbooks and orchestrate release activities
- Coordinate with operations and infrastructure teams
- Monitor deployments and trigger rollback if needed
- Document deployment outcomes and lessons learned

### Goals
- Achieve zero-downtime deployments
- Minimize deployment-related incidents
- Reduce time from code complete to production
- Maintain comprehensive deployment documentation

### Typical Communication
- Pre-deployment planning meetings with technical teams
- Release day coordination and status updates
- Post-deployment reports and retrospectives
- Escalation procedures for deployment issues

### Interactions with Other Roles
- **Project Managers**: Aligns deployment schedules with project timelines, reports on deployment status
- **QA Lead**: Validates release readiness, executes smoke tests, confirms quality gates
- **Developers**: Reviews deployment procedures, supports troubleshooting, coordinates hotfixes
- **Change Manager**: Submits change requests, ensures proper approvals, documents changes

---

## External Stakeholder

### Role Summary
External Stakeholders represent customer, partner, or vendor interests in the project. They provide input on requirements, validate solutions, offer feedback, and stay informed of project progress and decisions.

### Responsibilities
- Provide business context and requirements input
- Review and validate proposed solutions
- Participate in demos and feedback sessions
- Approve deliverables that impact their area
- Communicate organizational constraints and dependencies
- Stay informed of project status and key decisions

### Goals
- Ensure project outcomes meet organizational needs
- Maintain alignment between project and business objectives
- Provide timely feedback and approvals
- Minimize surprises and last-minute changes

### Typical Communication
- Monthly project status updates and demos
- Requirement validation sessions
- Approval workflows for major milestones
- Ad-hoc consultations for key decisions

### Interactions with Other Roles
- **Product Managers**: Provides business requirements, validates product direction, prioritizes features
- **Business Analyst**: Participates in requirements gathering, validates documentation, supports UAT
- **Project Managers**: Reviews project status, provides feedback on timeline and scope, approves changes
- **QA Lead**: Participates in UAT, validates quality expectations, reports production issues

---

## Role Handoffs and Collaboration

### Requirements Phase
1. **External Stakeholder → Business Analyst**: Provides initial business needs and context
2. **Business Analyst → Product Manager**: Translates requirements into product vision and features
3. **Product Manager → Developers**: Defines acceptance criteria and prioritized backlog

### Development Phase
1. **Developers → QA Lead**: Submits features for testing with test notes
2. **QA Lead → Developers**: Reports defects and validates fixes
3. **Business Analyst → QA Lead**: Clarifies acceptance criteria and expected behavior

### Change and Deployment Phase
1. **Developers/Project Manager → Change Manager**: Submits change requests with impact analysis
2. **Change Manager → Deployment Coordinator**: Approves changes and coordinates release windows
3. **Deployment Coordinator → QA Lead**: Validates release readiness and coordinates smoke testing
4. **QA Lead → Project Manager**: Provides final quality sign-off for release

### Feedback and Validation Phase
1. **Deployment Coordinator → External Stakeholder**: Notifies of deployment completion
2. **External Stakeholder → Business Analyst**: Provides feedback and reports issues
3. **Business Analyst → Product Manager**: Documents feedback for backlog prioritization

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

