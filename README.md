## Hi there 👋

I'm user-3410. If you're here, it's because you want to know more about my job.

This is my path:

# 🚀 Professional Experience as an IT Developer

## 📚 Index
1. [Freelance Apps](#freelance-apps)
2. [In Companies](#in-companies)
   - [Travel Industry](#travel-industry)
   - [Pharmaceutical Company](#pharma-industry)
   - [AgroTech Industry](#agrotech-industry)
   - [BigFour Consulting Agency](#bigfour-consulting-agency)
   - [Consulting](#consulting)
   - [Public Sector](#public-sector)
4. [Current Projects](#current-projects)
   - [Working on My Own Apps and Projects](#working-on-my-own-apps-and-projects)
   - [Working on Content Creation About Project Management](#working-on-content-creation-about-project-management)

## Freelance Apps

1. **Data Analyst:** Dashboards with PowerBI for sales analysis (2020)
   - **Technology:** PowerBI, MySQL

2. **Software Architect:** Data processing app for the tourism sector (2021)
   - **Technology:** Django, PostgreSQL

3. **Software Engineer:** Web scraping app (2021)
   - **Technology:** Python, BeautifulSoup, Selenium, AWS 🕸️

4. **Project Manager:** Company management app for Real Estate (2023)
   - **Technology:** Flask, Python, PostgreSQL

5. **Software Engineer:** Data analysis and integration app for the insurance sector (2024)
   - **Technology:** Python, PostgreSQL, FastAPI

## In Companies

### ✈️ Travel Industry (2025)

1. **Software Engineer:** Maintaining internal applications
   - **Technology:** Python, Django, Falcon, MongoDB, PostgreSQL, Azure, Scrum

### 💊 Pharma Industry (2024)

1. **Software Engineer and Solutions Architect:** Semantic Search of Clinical Trial and Pharma Teams
   - **Technology:** Python, FastAPI, Openshift, Opensearch, AWS, BitBucket, DevOps, Scrum

### 🌾 AgroTech Industry (2023)

1. **Software Engineer:** Desktop app for satellite image analysis
   - **Technology:** Python, PyQT, OpenCV, Docker, GitLab, Scrum

2. **Software Engineer:** Desktop app for satellite data analysis
   - **Technology:** Python, PostgreSQL, AWS, Tkinter, Docker, GitLab, Scrum

3. **Software Engineer:** API for satellite data uploading and processing
   - **Technology:** Python, FastAPI, PostgreSQL, AWS, GitLab, Scrum

4. **Software Engineer:** API for data cleaning
   - **Technology:** Symfony, PostgreSQL, Docker, GitLab, Scrum

### 💼 BigFour Consulting Agency (2021-2022)

1. **Software Engineer:** Payment processing software for an energy sector company
   - **Technology:** Django REST, PostgreSQL, Angular, Azure, GitHub, Scrum

2. **Software Engineer:** SaaS for logistics sector data analysis
   - **Technology:** Django REST, Azure, Docker, GitHub, Scrum

### 🧩 Consulting (2018-2020)

1. **Data Analyst and Process Analyst:** Dashboards for marketing data, data collection
   - **Technology:** Excel, PowerBI, R, Python

## 🏛️ Public Sector (2016-2019)

## Supreme Court:

1. **Software Engineer:** Application for the reception and tracking of criminal complaints (2019)
   - **Technology:** Laravel, Vue.js, MySQL, GitHub, Scrum

### Previous side projects in Supreme Court:

1. **Software Engineer:** WebApp for managing documents related to ISO 9001 quality certification (2018)
   - **Technology:** Django, PostgreSQL, GitHub

2. **Data Analyst:** Database integration and analysis for investigations related to money laundering, fraud and financial crimes (2018)
   - **Technology:** MySQL, Python, GitHub

3. **Data Analyst:** Financial Budget Planning Dashboards (2017)
   - **Technology:** MySQL, PHP, JavaScript

4. **Software Engineer:** Developed a system to consolidate mobile phone data usage for public officers (2016)
   - **Technology:** Laravel

## Current Projects

### 🌟 Working on My Own Apps and Projects (updates in August 2024)

1. **GenAI**
   - **Technology:** GCP, Python, FastAPI, Next.js

## Status:

👉 Currently focused on Software Architecture, MCP, and the development of applications with LLM agents.



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

#### Service Level Agreement and Format
- **Review Service Level Agreement:** Maximum 48 business hours
- **Feedback format:** Constructive, specific, and actionable
- **Communication:** When creating a PR, developer must inform reviewers explaining the changes made

#### Rejection Criteria
A PR can only be rejected for:
- Efficiency issues
- Security concerns
- Incompatibility with user story
- Scalability problems
- Lack of documentation

**Important note:** Code style rejections must be justified and should not introduce unnecessary delays. If code solves a critical user-impacting problem, security or efficiency, it should be deployed while minor aspects are refined.

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
- **Professional focus:** Work matters only, avoid personal topics and jokes

#### Communication Style
Given the multicultural nature of the team, a uniform communication style is established:
- **Clarity:** Use simple and direct language, avoid idioms or colloquial expressions
- **Assertiveness:** Express ideas and opinions directly but respectfully
- **Confirmation:** Request confirmation of understanding when dealing with complex topics
- **Patience:** Allow additional time for clarifications when necessary
- **Documentation:** Follow up important conversations with written summaries to avoid misunderstandings. Use AI.

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

