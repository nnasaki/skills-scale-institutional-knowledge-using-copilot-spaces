# OctoAcme — Role Assignment Guide

## Purpose
This guide helps project managers and team leads quickly identify which roles are needed for a project and ensure proper role coverage without overlap or gaps.

## Role Selection Decision Tree

### Always Required
- **Project Manager**: For any project (regardless of size)
- **Product Manager**: To define outcomes and prioritize
- **Developers**: To implement the solution

### Conditionally Required

#### Include UX Designer when:
- Building new user-facing features or experiences
- Redesigning existing user interfaces
- Conducting user research or usability testing
- Establishing or updating design systems
- Accessibility is a key requirement

#### Include DevOps Engineer when:
- Setting up new infrastructure or environments
- Implementing CI/CD pipelines
- Significant changes to deployment processes
- Performance, scalability, or reliability are critical concerns
- Infrastructure as Code is needed
- Complex monitoring or alerting setup required

#### Include QA Lead when:
- Quality strategy needs to be established or revised
- Multiple testing streams need coordination
- Test automation framework needs to be implemented
- Risk-based testing approach is needed
- Quality metrics and reporting are critical
- Team size requires dedicated quality coordination

**Note**: For smaller projects, QA responsibilities might be shared among developers with Product Manager oversight, but having a dedicated QA Lead is recommended for medium to large projects.

## Role Coverage Matrix

| Project Size | Typical Roles | Notes |
|--------------|--------------|-------|
| **Small** (1-2 sprints, 1-3 developers) | PM, PdM, Developers | Consider QA Lead; UX/DevOps as needed |
| **Medium** (3-6 sprints, 4-8 developers) | PM, PdM, Developers, QA Lead, DevOps | UX Designer strongly recommended |
| **Large** (6+ sprints, 8+ developers) | All roles | Multiple people may fill same role type |

## Preventing Role Ambiguity

### Common Ambiguity Points

#### "Who owns quality?"
- **Primary**: QA Lead defines quality strategy and gates
- **Shared**: Developers own unit test coverage
- **Oversight**: Product Manager defines acceptance criteria
- **Resolution**: Use Definition of Done as shared agreement

#### "Who decides on technical architecture?"
- **Primary**: Senior Developers / Tech Lead
- **Consulted**: DevOps Engineer (infrastructure), QA Lead (testability)
- **Informed**: Product Manager, Project Manager
- **Resolution**: Document decisions in Architecture Decision Records (ADRs)

#### "Who prioritizes bugs vs features?"
- **Primary**: Product Manager
- **Consulted**: QA Lead (bug severity/impact), Project Manager (capacity)
- **Informed**: Developers, stakeholders
- **Resolution**: Use clear severity/priority framework

#### "Who designs the user experience?"
- **Primary**: UX Designer
- **Consulted**: Product Manager (requirements), Developers (feasibility)
- **Informed**: QA Lead (test implications), Project Manager (timeline)
- **Resolution**: Design review process with clear approval gates

#### "Who decides deployment timing?"
- **Primary**: Product Manager + Project Manager (joint decision)
- **Consulted**: DevOps Engineer (readiness), QA Lead (quality), Developers (completeness)
- **Informed**: Stakeholders
- **Resolution**: Use deployment checklist and go/no-go criteria

#### "Who manages project risks?"
- **Primary**: Project Manager
- **Contributed**: All roles identify and report risks
- **Escalated**: Product Manager + Sponsor for high-impact risks
- **Resolution**: Maintain shared risk register, review weekly

## Role Overlap Best Practices

### Healthy Overlap
Some overlap is beneficial for collaboration:
- Developers and QA Lead both care about testability
- UX Designer and Product Manager both research users
- DevOps Engineer and Developers both care about code quality
- Project Manager and Product Manager both track progress

### Unhealthy Overlap (Anti-patterns)
Avoid these scenarios:
- ❌ Two people making conflicting priority decisions
- ❌ Duplicate work on same deliverable without coordination
- ❌ Multiple conflicting quality standards
- ❌ Parallel design efforts without alignment
- ❌ Competing technical architecture proposals without resolution

### How to Address Overlap Issues
1. **Clarify**: Reference this guide and the [Role Collaboration Matrix](./octoacme-role-collaboration-matrix.md)
2. **Communicate**: Hold quick sync between conflicting parties
3. **Document**: Capture decision and rationale
4. **Escalate**: If unresolved, bring to Project Manager or sponsor

## Role Assignment Checklist

When starting a new project:

### Step 1: Identify Core Roles
- [ ] Project Manager identified and available
- [ ] Product Manager identified and committed
- [ ] Developer(s) identified with required skills
- [ ] Confirm availability and capacity for all core roles

### Step 2: Assess Need for Specialized Roles
- [ ] Evaluate need for UX Designer (use decision tree above)
- [ ] Evaluate need for DevOps Engineer (use decision tree above)
- [ ] Evaluate need for QA Lead (use decision tree above)
- [ ] Document why each specialized role is/isn't included

### Step 3: Define Responsibilities
- [ ] Review [Roles and Personas](./octoacme-roles-and-personas.md) with team
- [ ] Clarify any role-specific expectations for this project
- [ ] Identify and document any deviations from standard roles
- [ ] Ensure everyone understands collaboration points

### Step 4: Set Up Communication
- [ ] Review [Role Collaboration Matrix](./octoacme-role-collaboration-matrix.md)
- [ ] Schedule regular syncs based on role interactions
- [ ] Establish decision-making protocols
- [ ] Set up shared tools and access

### Step 5: Document and Share
- [ ] Fill in "Proposed team / roles" in Project One-pager
- [ ] Add role-specific notes to project README
- [ ] Share role assignments with all stakeholders
- [ ] Add to onboarding materials for new team members

## Common Project Types and Recommended Role Setups

### New Product Feature
**Recommended**: PM, PdM, Developers, UX Designer, QA Lead, DevOps Engineer
**Why**: Full cross-functional team for quality and user experience

### API or Backend Service
**Recommended**: PM, PdM, Developers, DevOps Engineer, QA Lead
**Optional**: UX Designer (if developer experience is priority)

### Infrastructure Project
**Recommended**: PM, PdM, DevOps Engineer, Developers (infrastructure-focused)
**Optional**: QA Lead (for automation testing)

### Design System / Component Library
**Recommended**: PM, PdM, UX Designer, Developers (frontend), QA Lead
**Why**: Heavy design and frontend focus

### Bug Fix / Maintenance Sprint
**Recommended**: PM (light coordination), Developers, QA Lead
**Optional**: PdM oversight, DevOps (if infrastructure issues)

### Proof of Concept / Prototype
**Minimum**: PdM, Developer(s)
**Optional**: UX Designer (for user-facing PoC), PM (for multi-week efforts)

## Quick Reference: "Who Should I Talk To?"

| I need to... | Primary Role | Secondary Role |
|-------------|--------------|----------------|
| Clarify feature requirements | Product Manager | UX Designer |
| Understand project timeline | Project Manager | - |
| Discuss technical approach | Developer / Tech Lead | DevOps Engineer |
| Review design mockups | UX Designer | Product Manager |
| Report a blocker | Project Manager | Product Manager |
| Validate quality standards | QA Lead | Product Manager |
| Plan deployment | DevOps Engineer | Project Manager |
| Get production access | DevOps Engineer | Project Manager |
| Understand test strategy | QA Lead | Developers |
| Propose architecture change | Tech Lead / Senior Dev | DevOps Engineer |
| Escalate a risk | Project Manager | Product Manager |
| Request design resources | UX Designer | Project Manager |

---

*Use this guide in conjunction with [Roles and Personas](./octoacme-roles-and-personas.md) and [Role Collaboration Matrix](./octoacme-role-collaboration-matrix.md) for comprehensive role management.*
