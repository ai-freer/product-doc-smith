# Experiment PRD

## Experiment PRD

### Experiment Overview

**Experiment Name**
[Concise experiment name]

**Experiment Hypothesis**
*"If we [change/intervention], then [expected outcome] will happen because of [reason]."*

**Experiment Type**
[ ] A/B Test
[ ] Multivariate Test
[ ] Prototype Test
[ ] Pilot Program
[ ] Landing Page Test
[ ] Other: [Specify]

**Primary Success Metric**
[Metric name] - Target: [X% improvement/change]

**Secondary Metrics**
1. [Metric 1] - Target: [Target]
2. [Metric 2] - Target: [Target]

**Guardrail Metrics**
1. [Metric 1] - Unacceptable threshold: [Threshold]
2. [Metric 2] - Unacceptable threshold: [Threshold]

---

### Context & Rationale

**What problem are we trying to solve?**
Describe the problem or opportunity that this experiment addresses.

**Why do we need to test this?**
Explain why we can't just launch this without testing. What's uncertain?

**What assumptions are we testing?**
List the key assumptions underlying this experiment.

**Previous Learnings**
What have we learned from previous experiments or research that informs this one?

---

### Success Criteria

**Primary Criteria**
The experiment is successful if:
- [Success criteria 1]
- [Success criteria 2]

**Failure Criteria**
The experiment is considered a failure if:
- [Failure criteria 1]
- [Failure criteria 2]

**Minimum Detectable Effect (MDE)**
- For primary metric: [X%]
- Power level: [X%]
- Significance level: [X%]

**Statistical Significance**
- Target confidence level: [X%]
- Minimum sample size: [N users]

---

### Experiment Design

**Control Group**
Describe the baseline or control condition.
- [ ] Existing solution/feature
- [ ] No change
- [ ] Other: [Specify]

**Treatment Group(s)**
Describe the variation(s) being tested.
- Variant A: [Description]
- Variant B: [Description] (if applicable)

**Experiment Logic**
[Describe the logic/rule that determines which users see which variant]

**Randomization**
[Describe how users are assigned to groups]

**Duration**
- Start date: [Date]
- End date: [Date]
- Total duration: [X] days

**Traffic Allocation**
- Control: [X]%
- Variant A: [X]%
- Variant B: [X]% (if applicable)

---

### Implementation

**Feature/Change Description**
[Detailed description of what's being implemented for each variant]

**Technical Requirements**
- [ ] Backend changes: [Description]
- [ ] Frontend changes: [Description]
- [ ] Data tracking: [Description]
- [ ] Infrastructure: [Description]

**Data Tracking**
**Key Events to Track**
1. [Event 1] - Definition: [Description]
2. [Event 2] - Definition: [Description]

**Required Attributes**
- [Attribute 1]: [Type]
- [Attribute 2]: [Type]

**Dashboard/Reporting**
- Dashboard link: [URL]
- Reporting frequency: [Daily/Weekly]

---

### Target Audience

**Who is being tested?**
- Target user segment: [Description]
- Eligibility criteria: [Criteria]
- Total eligible users: [N]

**Exclusion Criteria**
Who should NOT be included in the experiment?
- [Exclusion 1]
- [Exclusion 2]

**Sample Size Calculation**
- Required sample size: [N users]
- Traffic required: [X% of total]
- Time to reach sample size: [X days/weeks]

---

### Risk Assessment

**Risks to Users**
| Risk | Likelihood | Impact | Mitigation |
|------|-----------|--------|------------|
| [Risk 1] | High/Med/Low | High/Med/Low | [Strategy] |

**Risks to Business**
| Risk | Likelihood | Impact | Mitigation |
|------|-----------|--------|------------|
| [Risk 1] | High/Med/Low | High/Med/Low | [Strategy] |

**Kill Switches**
- [ ] Can we stop the experiment immediately? Yes/No
- [ ] How do we stop it? [Procedure]

---

### Analysis Plan

**Primary Analysis Method**
[Describe how you'll analyze the primary metric]

**Statistical Tests**
- [ ] T-test
- [ ] Chi-square test
- [ ] Z-test
- [ ] Other: [Specify]

**Segmentation Analysis**
Do you plan to analyze results by segment?
- Segment 1: [Description]
- Segment 2: [Description]

**Success/Failure Decision Rules**
- **Success**: [Criteria]
- **Failure**: [Criteria]
- **Inconclusive**: [Criteria]

---

### Timeline & Milestones

**Pre-Experiment**
- [ ] [Date]: Finalize experiment design
- [ ] [Date]: Implement feature/change
- [ ] [Date]: QA and testing
- [ ] [Date]: Launch experiment

**During Experiment**
- [ ] [Date]: First data review
- [ ] [Date]: Mid-point check
- [ ] [Date]: Final data collection

**Post-Experiment**
- [ ] [Date]: Analyze results
- [ ] [Date]: Make Go/No-Go decision
- [ ] [Date]: Share learnings

---

### Decision Framework

**If Successful: Next Steps**
- [ ] Launch to [X]% of users
- [ ] Full rollout
- [ ] Iterate and retest
- [ ] Other: [Describe]

**If Failed: Next Steps**
- [ ] Abandon feature
- [ ] Iterate and retest
- [ ] Learn and apply elsewhere
- [ ] Other: [Describe]

**If Inconclusive: Next Steps**
- [ ] Extend experiment
- [ ] Run with larger sample
- [ ] Redesign experiment
- [ ] Other: [Describe]

---

### Team & Responsibilities

**Experiment Owner**
[Name] - [Role] - [Contact]

**Stakeholders**
- [Stakeholder 1] - [Role]
- [Stakeholder 2] - [Role]

**Required Approvals**
- [ ] Product: [Name] - Approved by: [Date]
- [ ] Engineering: [Name] - Approved by: [Date]
- [ ] Data Science: [Name] - Approved by: [Date]
- [ ] Legal/Compliance: [Name] - Approved by: [Date] (if applicable)

---

### Appendix

**Technical Documentation**
[Link to technical specs]

**Data Definitions**
[Metric definitions and formulas]

**Related Experiments**
- [Previous experiment 1]: [Link]
- [Related experiment 2]: [Link]

**Learnings Log**
[Document key learnings as experiment progresses]
