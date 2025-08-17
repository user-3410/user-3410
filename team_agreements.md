# Team Working Agreements

## 1. Technical Governance and Roles

### 1.1 Responsibility Matrix (RACI)

| Component | Primary Responsible | Approver | Consulted | Informed |
|-----------|-------------------|----------|-----------|----------|
| Backend (FastAPI) | Backend Engineer | Technical Architect | Frontend, DevOps | Full Team |
| Frontend (Angular) | Frontend Engineer | Technical Architect | Backend, UX/UI | Full Team |
| Infrastructure (OpenShift) | DevOps Engineer | Tech Lead | Backend, Frontend | Full Team |
| Data & Search (OpenSearch) | Data Engineer | Technical Architect | Backend | Full Team |
| Global Architecture | Technical Architect | Tech Lead | All Responsible Parties | Stakeholders |

### 1.2 Decision-Making Process

#### Single Component Decisions
- Component owner (Backend, Frontend, Data Engineer, etc.) decides after internal consultation
- Maximum consultation time: 48 business hours
- Mandatory documentation in corresponding technical channel

#### Architectural Decisions
- Require documented consensus among technical leads
- Escalation process to technical committee if no consensus within 5 business days
- All decisions must be recorded as ADRs (Architecture Decision Records)

## 2. Development Standards and Quality

### 2.1 Definition of Done

**Prerequisites before implementation:**
- [ ] Technical documentation created
- [ ] Solution discussion and approval (functionality, security, scalability, efficiency)
- [ ] Schemas and flow diagrams documented
- [ ] Business core and main functions defined

**During development:**
- [ ] Code reviewed and approved by component owner
- [ ] Test coverage:
  - 95% for business-critical functions
  - 80% for non-critical functions
- [ ] Automated linting and formatting applied (Black formatter, SonarLint)
- [ ] Security review completed (for critical changes)

**After implementation:**
- [ ] Technical documentation updated
- [ ] Video recording explaining critical functions and technical decisions

### 2.2 Code Review Process

#### SLA and Format
- **Review SLA:** Maximum 48 business hours
- **Feedback format:** Constructive, specific, and actionable
- **Communication:** When creating a PR, developer must inform reviewers explaining the changes made

#### Rejection Criteria
A PR can only be rejected for:
- Efficiency issues
- Security concerns
- Incompatibility with user story
- Scalability problems
- Lack of documentation

**Important note:** Code style rejections must be justified and should not introduce unnecessary delays. If code solves a critical user-impacting problem, it should be deployed while minor aspects are refined.

#### Required Approvals
1. **Mandatory:** 1 approval from component owner
2. **For architectural changes:** 1 additional approval
3. **For critical changes:** Video session explaining changes and rationale

## 3. Communication and Collaboration

### 3.1 Meeting Structure

#### Daily Standup (15 min max)
- **Format:** What did I do yesterday? What will I do today? What's blocking me?
- **Focus:** Only blockers and critical dependencies
- **Rule:** Detailed technical conversations are deferred

#### Weekly Technical Review (45 min max)
- **Prerequisite:** Agenda sent 24 hours in advance
- **Limit:** Maximum 3 technical topics per session
- **Documentation:** Decisions recorded in real-time

#### Technical Refinement (1 hour per sprint)
- Technical complexity analysis of new stories
- Identification of component dependencies
- Technical effort estimation

### 3.2 Asynchronous Communication

- **Standard response time:** 24 business hours
- **Specialized channels:** By component (#backend, #frontend, #infra, #data)
- **Centralized documentation:** Technical wiki updated weekly

#### Meeting Guidelines
- **Mandatory prior notification:** Include agenda and topics to be discussed
- **Camera mandatory:** Keep camera on during all meetings
- **Objective:** Facilitate productive and focused discussions
- **Professional focus:** Work matters only, avoid personal topics

#### Communication Style
Given the multicultural nature of the team, a uniform communication style is established:
- **Clarity:** Use simple and direct language, avoid idioms or colloquial expressions
- **Assertiveness:** Express ideas and opinions directly but respectfully
- **Confirmation:** Request confirmation of understanding when dealing with complex topics
- **Patience:** Allow additional time for clarifications when necessary
- **Documentation:** Follow up important conversations with written summaries to avoid misunderstandings

## 4. Work Planning and Management

### 4.1 Definition of Ready for User Stories

- [ ] Clear and measurable acceptance criteria
- [ ] Technical analysis completed (for complex stories)
- [ ] Dependencies identified and documented
- [ ] Agreed effort estimation
- [ ] Mockups/wireframes available (if applicable)
- [ ] Test criteria defined
- [ ] Security criteria defined
- [ ] Efficiency criteria defined
- [ ] QA testing methodology specified

### 4.2 Technical Debt Management

- **Time allocation:** 20% of sprint dedicated to technical improvements
- **Prioritization:** Based on impact on performance, scalability, and maintainability
- **Registry:** Centralized backlog with impact metrics
- **Review:** Monthly session to evaluate and prioritize technical debt

## 5. Metrics and Continuous Improvement

### 5.1 Key Performance Indicators (KPIs)

- **Average PR review time:** < 24 hours
- **Production defect rate:** < 2% per sprint
- **Test coverage:** > 80% consistently maintained
- **Blocker resolution time:** < 48 hours
- **Team satisfaction:** Monthly measurement (1-5 scale)
- **Fitness Functions:** Load evaluation from end-user perspective

### 5.2 Retrospectives

- **Frequency:** Every 2 sprints
- **Structured format:** Start/Stop/Continue with specific actions
- **Follow-up:** Review action implementation in next retrospective
- **Analysis:** Include KPIs and team trends

## 6. Conflict Resolution and Escalation

### Escalation Process
1. **Level 1:** Direct discussion between parties (48 hours maximum)
2. **Level 2:** Tech Lead mediation (72 hours maximum)
3. **Level 3:** Technical committee (Architect + 2 rotating seniors)

## 7. Knowledge Sharing

- **Monthly Tech Talks:** Rotating technical presentations (30 min)
- **Mandatory documentation:** For all architectural decisions
- **Pair programming:** Minimum 2 hours weekly between different components
- **Task rotation:** Quarterly to improve complete system understanding

---

*These agreements will be reviewed quarterly and updated based on team needs and lessons learned.*
