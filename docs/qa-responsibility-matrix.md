# QA Responsibility Matrix

## Purpose
This matrix defines quality assurance responsibilities across different project phases and team roles. It clarifies who is responsible, accountable, consulted, and informed (RACI) for various quality-related activities, reducing ambiguity and improving cross-functional collaboration.

---

## RACI Legend

- **R (Responsible)**: Person who performs the work to complete the task
- **A (Accountable)**: Person who is ultimately answerable for the correct completion of the task
- **C (Consulted)**: Person whose input is sought; two-way communication
- **I (Informed)**: Person who is kept up-to-date on progress; one-way communication

---

## Quality Assurance Activities Matrix

### Requirements and Planning Phase

| Activity | QA Lead | Developer | Product Manager | Business Analyst | Project Manager |
|----------|---------|-----------|-----------------|------------------|-----------------|
| Define testability requirements | R | C | C | C | I |
| Review acceptance criteria | R | C | A | C | I |
| Create test strategy | A/R | C | C | I | I |
| Estimate testing effort | A/R | C | I | I | C |
| Define test environment needs | R | C | I | I | A |
| Identify quality metrics | A/R | C | C | I | C |
| Review risk assessment for quality impacts | R | I | C | I | A |
| Define Definition of Done (DoD) | R | R | A | C | C |

### Development Phase

| Activity | QA Lead | Developer | Product Manager | Business Analyst | Project Manager |
|----------|---------|-----------|-----------------|------------------|-----------------|
| Unit test creation | I | A/R | I | I | I |
| Code review for testability | C | A/R | I | I | I |
| Integration test design | A/R | C | I | I | I |
| Test case creation | A/R | C | C | C | I |
| Test data preparation | R | C | I | I | I |
| Execute functional testing | A/R | I | I | I | I |
| Execute regression testing | A/R | I | I | I | I |
| API/service testing | R | C | I | I | I |
| Performance testing | R | C | I | I | I |
| Security testing coordination | R | C | I | I | A |

### Defect Management

| Activity | QA Lead | Developer | Product Manager | Business Analyst | Project Manager |
|----------|---------|-----------|-----------------|------------------|-----------------|
| Defect identification | R | R | I | I | I |
| Defect logging and documentation | R | R | I | I | I |
| Defect triage and prioritization | A | R | C | C | C |
| Defect assignment | A | I | I | I | C |
| Root cause analysis | C | A/R | I | I | I |
| Defect fix verification | A/R | I | I | I | I |
| Regression test execution | A/R | I | I | I | I |
| Track defect metrics | A/R | I | C | I | C |

### User Acceptance Testing (UAT)

| Activity | QA Lead | Developer | Product Manager | Business Analyst | Project Manager |
|----------|---------|-----------|-----------------|------------------|-----------------|
| UAT planning | R | I | C | A | C |
| UAT environment setup | R | C | I | I | I |
| UAT test case preparation | C | I | A | R | I |
| UAT coordination | R | I | C | C | A |
| UAT execution support | R | C | I | C | I |
| UAT defect triage | A | R | C | C | C |
| UAT sign-off facilitation | R | I | C | A | C |

### Release and Deployment

| Activity | QA Lead | Developer | Product Manager | Business Analyst | Deployment Coordinator | Project Manager |
|----------|---------|-----------|-----------------|------------------|------------------------|-----------------|
| Pre-release testing | A/R | I | I | I | C | I |
| Smoke test preparation | A/R | C | I | I | C | I |
| Release readiness sign-off | R | I | I | I | C | A |
| Deployment smoke testing | A/R | C | I | I | C | I |
| Production validation | A/R | C | I | I | I | I |
| Post-deployment monitoring | R | C | I | I | R | C |
| Rollback testing (if needed) | R | R | I | I | A | C |

### Continuous Quality Improvement

| Activity | QA Lead | Developer | Product Manager | Business Analyst | Project Manager |
|----------|---------|-----------|-----------------|------------------|-----------------|
| Quality metrics reporting | A/R | I | C | I | C |
| Test automation strategy | A/R | C | I | I | I |
| Test process improvement | A/R | C | I | I | C |
| Quality retrospective facilitation | R | R | I | I | A |
| Testing tools evaluation | A/R | C | I | I | I |

---

## Responsibility Guidelines by Role

### QA Lead Primary Responsibilities
- Own overall test strategy and execution
- Ensure quality gates are met before release
- Manage defect triage and resolution tracking
- Report quality metrics and risks
- Sign off on release readiness from quality perspective
- Drive continuous improvement in testing practices

### Developer Primary Responsibilities
- Write unit tests for all code changes
- Ensure code is testable and maintainable
- Fix defects in timely manner
- Support integration and system testing
- Participate in code reviews with quality focus
- Collaborate with QA on test automation

### Product Manager Primary Responsibilities
- Define clear acceptance criteria
- Prioritize defect fixes vs. new features
- Approve UAT sign-off
- Make trade-off decisions on quality vs. timeline
- Validate that quality meets customer expectations

### Business Analyst Primary Responsibilities
- Ensure acceptance criteria are testable
- Support UAT planning and execution
- Clarify requirements for test case creation
- Validate business logic in testing
- Bridge communication between QA and business stakeholders

### Project Manager Primary Responsibilities
- Ensure adequate time and resources for testing
- Track quality metrics against project goals
- Escalate quality risks to stakeholders
- Coordinate cross-team testing dependencies
- Approve release readiness from overall project perspective

### Deployment Coordinator Primary Responsibilities
- Coordinate release testing activities
- Validate deployment readiness checks
- Execute post-deployment smoke tests
- Monitor production deployment health
- Trigger rollback if quality issues detected

---

## Escalation Paths

### Quality Issues Escalation

1. **Minor Defects**: QA Lead → Developer → Resolved
2. **Major Defects**: QA Lead → Developer + Project Manager → Resolved or escalated
3. **Critical/Blocker Defects**: QA Lead → Project Manager + Product Manager → Immediate action
4. **Quality Gate Failures**: QA Lead → Project Manager → Product Manager → Decision on release
5. **Production Quality Issues**: QA Lead → Deployment Coordinator → Project Manager → Incident response

### Testing Timeline Issues

1. **At Risk**: QA Lead → Project Manager → Adjust plan
2. **Behind Schedule**: QA Lead + Project Manager → Product Manager → Prioritization decision
3. **Cannot Meet Release Date**: Project Manager → Product Manager → Stakeholders → Release decision

---

## Quality Gates and Sign-offs

### Quality Gate 1: Development Complete
- **Criteria**: All unit tests pass, code review complete, integration tests pass
- **Sign-off**: Developer (R), QA Lead (A)

### Quality Gate 2: Testing Complete
- **Criteria**: All test cases executed, critical defects resolved, regression tests pass
- **Sign-off**: QA Lead (A), Product Manager (C)

### Quality Gate 3: UAT Complete
- **Criteria**: UAT test cases pass, business validation complete, no blocking issues
- **Sign-off**: Business Analyst (R), Product Manager (A), QA Lead (C)

### Quality Gate 4: Release Ready
- **Criteria**: All quality gates passed, smoke tests ready, rollback plan validated
- **Sign-off**: QA Lead (R), Project Manager (A), Product Manager (C)

### Quality Gate 5: Production Validated
- **Criteria**: Smoke tests pass in production, monitoring shows healthy state, no critical issues
- **Sign-off**: Deployment Coordinator (R), QA Lead (C), Project Manager (A)

---

## Communication Cadence

### Daily
- **Standup**: QA Lead shares testing status, blockers, and defect triage updates
- **Defect Review**: QA Lead and Developers review new defects and prioritize fixes

### Weekly
- **Quality Metrics Review**: QA Lead shares metrics dashboard with Project Manager and Product Manager
- **Test Progress Review**: QA Lead and Project Manager review test execution progress vs. plan

### Sprint/Iteration
- **Sprint Planning**: QA Lead participates to estimate testing effort and identify testability concerns
- **Sprint Review**: QA Lead demos test results and quality metrics
- **Sprint Retrospective**: QA Lead shares testing process improvements

### Release Cycle
- **Pre-Release Review**: QA Lead, Project Manager, Product Manager review release readiness
- **Post-Release Review**: QA Lead facilitates review of production issues and quality metrics

---

## Key Deliverables by Phase

### Planning Phase Deliverables
- Test Strategy Document (QA Lead - R)
- Test Plan with Schedule (QA Lead - R, Project Manager - A)
- Test Environment Requirements (QA Lead - R)

### Execution Phase Deliverables
- Test Cases and Scripts (QA Lead - R)
- Test Execution Reports (QA Lead - R)
- Defect Reports and Metrics (QA Lead - R)
- Weekly Quality Status Report (QA Lead - R)

### Release Phase Deliverables
- Release Readiness Report (QA Lead - R)
- Smoke Test Results (QA Lead - R)
- Production Validation Report (QA Lead - R)

### Continuous Improvement Deliverables
- Quality Metrics Dashboard (QA Lead - R)
- Process Improvement Recommendations (QA Lead - R)
- Test Automation Coverage Report (QA Lead - R)

---

## Notes and Best Practices

- **Flexibility**: This matrix can be adapted for specific project needs while maintaining clear accountability
- **Communication**: When in doubt, over-communicate rather than assume someone else is responsible
- **Collaboration**: Quality is everyone's responsibility; this matrix clarifies specific accountabilities
- **Review Regularly**: Review and update this matrix at project kickoff and retrospectives
- **Tool Support**: Use project management tools to assign and track these responsibilities
- **Documentation**: Keep this matrix visible and accessible to all team members

---

*This QA Responsibility Matrix is part of the OctoAcme project management framework. For questions or suggestions, contact your QA Lead or Project Manager.*
