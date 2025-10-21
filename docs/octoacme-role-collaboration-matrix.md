# OctoAcme — Role Collaboration Matrix

## Purpose
This document clarifies how different roles interact throughout the project lifecycle to prevent ambiguity, avoid duplication of effort, and strengthen cross-functional collaboration.

## Collaboration Overview

### Product Manager ↔ Other Roles

| Role | Collaboration Points | Frequency | Key Artifacts |
|------|---------------------|-----------|---------------|
| Project Manager | Roadmap alignment, priority discussions, scope changes | Weekly sync | Roadmap, backlog priorities |
| Developers | Feature specs, acceptance criteria, technical feasibility | As needed | User stories, acceptance criteria |
| UX Designer | Problem validation, design decisions, user research findings | Bi-weekly + as needed | Research reports, design specs |
| DevOps Engineer | Performance requirements, infrastructure needs | Monthly + as needed | NFRs, SLAs |
| QA Lead | Quality requirements, acceptance criteria validation | Sprint planning | Test strategy, quality metrics |

### Project Manager ↔ Other Roles

| Role | Collaboration Points | Frequency | Key Artifacts |
|------|---------------------|-----------|---------------|
| Product Manager | Scope, timeline, resource allocation | Weekly sync | Project plan, status reports |
| Developers | Sprint planning, blockers, dependencies | Daily standups | Sprint backlog, burndown |
| UX Designer | Design timelines, review schedules | Sprint planning | Design milestones |
| DevOps Engineer | Infrastructure readiness, deployment planning | Weekly + as needed | Deployment plan, risk register |
| QA Lead | Test planning, quality gates, release criteria | Sprint planning + pre-release | Test plan, quality reports |

### Developer ↔ Other Roles

| Role | Collaboration Points | Frequency | Key Artifacts |
|------|---------------------|-----------|---------------|
| Product Manager | Clarify requirements, technical constraints | As needed | Technical design docs |
| UX Designer | Implementation feasibility, design handoff | Sprint start + as needed | Design specs, component library |
| DevOps Engineer | Deployment automation, build issues, monitoring | Daily + as needed | CI/CD configs, deployment docs |
| QA Lead | Testability, test coverage, bug triage | Daily + sprint reviews | Unit tests, integration tests |

### UX Designer ↔ Other Roles

| Role | Collaboration Points | Frequency | Key Artifacts |
|------|---------------------|-----------|---------------|
| Product Manager | User research, design validation, prioritization | Bi-weekly | Personas, journey maps, wireframes |
| Project Manager | Design timelines, resource needs | Sprint planning | Design roadmap |
| Developers | Design handoff, implementation review, feasibility | Sprint start + reviews | Design specs, style guide |
| QA Lead | Usability test plans, accessibility requirements | Sprint planning | Accessibility checklist, usability test scripts |

### DevOps Engineer ↔ Other Roles

| Role | Collaboration Points | Frequency | Key Artifacts |
|------|---------------------|-----------|---------------|
| Product Manager | Infrastructure requirements, performance SLAs | Monthly | NFRs, capacity plans |
| Project Manager | Infrastructure dependencies, deployment windows | Weekly | Deployment schedule, runbooks |
| Developers | CI/CD pipeline, build issues, environment setup | Daily | Pipeline configs, deployment guides |
| QA Lead | Test environment setup, automated test integration | Sprint planning | Test environments, CI/CD test stages |

### QA Lead ↔ Other Roles

| Role | Collaboration Points | Frequency | Key Artifacts |
|------|---------------------|-----------|---------------|
| Product Manager | Quality requirements, acceptance criteria | Sprint planning | Quality standards, test strategy |
| Project Manager | Quality status, test progress, release readiness | Weekly | Quality reports, defect metrics |
| Developers | Test coverage, testability, bug fixes | Daily | Test cases, defect reports |
| UX Designer | Usability testing, accessibility validation | Sprint reviews | Usability test results |
| DevOps Engineer | Test automation integration, production monitoring | Sprint planning | Automated test suites, quality dashboards |

## Communication Protocols

### Daily Touchpoints
- **Standups**: Developers, QA Lead, DevOps Engineer (15 min)
  - Yesterday's progress, today's plan, blockers

### Sprint-Level Touchpoints
- **Sprint Planning**: All roles (2-4 hours)
  - Backlog refinement, capacity planning, commitment
- **Sprint Review/Demo**: All roles + stakeholders (1 hour)
  - Demo completed work, gather feedback
- **Sprint Retrospective**: All delivery team members (1 hour)
  - Process improvements, action items

### Ongoing Collaboration
- **Design Reviews**: Product Manager, UX Designer, Developers (as needed)
- **Technical Reviews**: Developers, DevOps Engineer (as needed)
- **Quality Reviews**: QA Lead, Developers, Product Manager (pre-release)

## Decision-Making Authority

### Product Decisions
- **Owner**: Product Manager
- **Consulted**: UX Designer, Project Manager, key stakeholders
- **Informed**: All team members

### Technical Architecture
- **Owner**: Senior Developers / Tech Lead
- **Consulted**: DevOps Engineer, QA Lead
- **Informed**: Product Manager, Project Manager

### Design Decisions
- **Owner**: UX Designer
- **Consulted**: Product Manager, Developers (for feasibility)
- **Informed**: Project Manager, QA Lead

### Release Decisions (Go/No-Go)
- **Owner**: Project Manager + Product Manager (joint)
- **Consulted**: QA Lead, DevOps Engineer, Developers
- **Informed**: Stakeholders

### Infrastructure & Deployment
- **Owner**: DevOps Engineer
- **Consulted**: Developers, QA Lead
- **Informed**: Project Manager, Product Manager

### Quality Standards
- **Owner**: QA Lead
- **Consulted**: Product Manager, Developers
- **Informed**: Project Manager, stakeholders

## Escalation Paths

### Technical Blockers
1. Developer → Tech Lead → DevOps Engineer (if infrastructure)
2. If unresolved → Project Manager → Product Manager

### Design Conflicts
1. UX Designer ↔ Product Manager discussion
2. If unresolved → Include Project Manager → escalate to sponsor

### Quality/Risk Issues
1. QA Lead → Project Manager + Product Manager
2. If critical → Immediate stakeholder notification

### Resource/Timeline Conflicts
1. Project Manager → Product Manager → Sponsor/Stakeholders

## Onboarding Checklist for New Role Members

### For All Roles
- [ ] Read [Project Management Overview](./octoacme-project-management-overview.md)
- [ ] Review [Roles and Personas](./octoacme-roles-and-personas.md) for your role and collaborating roles
- [ ] Understand your role's decision-making authority
- [ ] Identify your key collaboration points and communication cadence
- [ ] Set up necessary tools and access
- [ ] Schedule introductions with key collaborators

### Role-Specific Onboarding

#### Developers
- [ ] Set up development environment
- [ ] Review coding standards and contribution guidelines
- [ ] Get access to CI/CD pipelines and deployment tools
- [ ] Review architectural documentation

#### UX Designers
- [ ] Access design tools and design system
- [ ] Review existing user research and personas
- [ ] Understand design review process
- [ ] Connect with Product Manager on current priorities

#### DevOps Engineers
- [ ] Get infrastructure access and credentials
- [ ] Review deployment procedures and runbooks
- [ ] Understand monitoring and alerting setup
- [ ] Review incident response procedures

#### QA Leads
- [ ] Access test management tools
- [ ] Review test strategy and coverage
- [ ] Understand quality gates and release criteria
- [ ] Set up test environments

#### Product Managers
- [ ] Review product roadmap and backlog
- [ ] Understand user personas and target market
- [ ] Review success metrics and KPIs
- [ ] Connect with key stakeholders

#### Project Managers
- [ ] Review project charter and timeline
- [ ] Understand risk register and dependencies
- [ ] Set up project tracking tools
- [ ] Schedule regular syncs with all key roles

## Best Practices

### Preventing Role Ambiguity
1. **Clear RACI**: Use RACI (Responsible, Accountable, Consulted, Informed) for major decisions
2. **Document Agreements**: Capture decisions and action items in shared spaces
3. **Regular Syncs**: Maintain communication cadence to surface issues early
4. **Explicit Handoffs**: Clearly communicate when work moves between roles

### Avoiding Duplication
1. **Single Source of Truth**: Maintain one canonical location for key artifacts
2. **Role Boundaries**: Respect decision-making authority outlined above
3. **Transparency**: Share work-in-progress to avoid parallel efforts
4. **Backlog Grooming**: Regular backlog refinement to prevent duplicate work items

### Strengthening Collaboration
1. **Cross-Functional Pairing**: Encourage pairing across roles (e.g., Developer + UX Designer)
2. **Shared Goals**: Align on common success metrics
3. **Psychological Safety**: Create environment for questions and feedback
4. **Celebrate Wins**: Recognize collaborative achievements

---

*This collaboration matrix is a living document. Update it as team structure and processes evolve.*
