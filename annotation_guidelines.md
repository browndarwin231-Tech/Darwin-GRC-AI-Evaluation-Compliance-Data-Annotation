# AI GRC Annotation Guidelines

## Purpose

These guidelines define how simulated AI-generated Governance, Risk, and Compliance responses should be reviewed, labeled, scored, and documented.

The goal is to create a consistent evaluation process for AI responses involving security frameworks, compliance requirements, risk statements, control mappings, audit evidence, and remediation recommendations.

---

## Reviewer Responsibilities

The reviewer should:

- Read the full scenario
- Identify the relevant framework
- Review the AI-generated response
- Check factual accuracy
- Check completeness
- Evaluate reasoning quality
- Review control mappings
- Identify unsupported claims
- Assess remediation quality
- Assign a label
- Assign numerical scores
- Document reviewer comments
- Provide an improved response when needed

---

## Evaluation Labels

### Accurate

Use when the response is factually correct, complete, relevant, and appropriately aligned with the framework.

### Mostly Accurate

Use when the response is generally correct but contains minor omissions or limited detail.

### Incomplete

Use when the response contains useful information but misses important requirements, risks, controls, evidence, or context.

### Incorrect

Use when the response contains significant factual errors or applies the wrong framework, control, or requirement.

### Unsupported

Use when the response makes claims that are not supported by the scenario, available evidence, or framework guidance.

### Needs Human Review

Use when the scenario is ambiguous, high-risk, legally sensitive, or requires additional subject-matter expertise before a final decision can be made.

---

## Scoring Criteria

Each response should receive scores from 1 to 5.

### Accuracy Score

| Score | Description |
|---|---|
| 5 | Fully accurate |
| 4 | Mostly accurate with minor issues |
| 3 | Partially accurate |
| 2 | Significant inaccuracies |
| 1 | Incorrect or misleading |

### Completeness Score

| Score | Description |
|---|---|
| 5 | Covers all important elements |
| 4 | Minor omissions |
| 3 | Several important details missing |
| 2 | Major gaps |
| 1 | Does not adequately address the scenario |

### Reasoning Score

| Score | Description |
|---|---|
| 5 | Clear, logical, and well-supported reasoning |
| 4 | Good reasoning with minor weaknesses |
| 3 | Basic reasoning but limited explanation |
| 2 | Weak or inconsistent reasoning |
| 1 | No meaningful reasoning |

### Framework Alignment Score

| Score | Description |
|---|---|
| 5 | Strong alignment with applicable framework |
| 4 | Mostly aligned with minor issues |
| 3 | Partial alignment |
| 2 | Significant mapping problems |
| 1 | Wrong framework or requirement |

### Remediation Quality Score

| Score | Description |
|---|---|
| 5 | Specific, realistic, measurable, and relevant |
| 4 | Strong recommendation with minor omissions |
| 3 | General but usable recommendation |
| 2 | Weak or incomplete recommendation |
| 1 | Incorrect or impractical recommendation |

---

## Annotation Decision Process

For each record:

1. Identify the framework
2. Identify the control or compliance topic
3. Read the AI response
4. Compare the response to the scenario
5. Identify correct statements
6. Identify missing information
7. Identify incorrect statements
8. Identify unsupported assumptions
9. Review control mapping
10. Review risk interpretation
11. Evaluate recommended remediation
12. Assign the final label
13. Assign numerical scores
14. Write reviewer comments
15. Provide an improved response if necessary

---

## Accuracy Review

The reviewer should determine whether the AI response:

- Uses the correct framework
- Uses appropriate control concepts
- Avoids inventing requirements
- Distinguishes guidance from mandatory requirements
- Correctly describes risk
- Correctly describes evidence
- Avoids unsupported legal conclusions
- Avoids overgeneralizing framework expectations

---

## Completeness Review

Check whether the response addresses:

- Control objective
- Current state
- Gap
- Risk
- Business impact
- Evidence
- Responsible owner
- Remediation
- Validation
- Follow-up

Not every scenario requires all of these elements, but the reviewer should identify material omissions.

---

## Control Mapping Review

A control mapping should be considered acceptable when:

- The control relates directly to the scenario
- The control objective addresses the identified risk
- The mapping is not based only on keyword similarity
- The response explains why the control applies

A weak mapping may:

- Use the wrong control family
- Map an unrelated control
- Ignore the actual risk
- Provide no explanation
- Treat different frameworks as identical

---

## Risk Statement Review

A strong risk statement should identify:

**Cause → Risk Event → Business Impact**

Example:

Weak:

> MFA is missing.

Improved:

> Incomplete MFA coverage may allow compromised credentials to be used for unauthorized access, increasing the risk of data exposure or system compromise.

---

## Evidence Review

The reviewer should evaluate whether requested evidence would reasonably support the control.

Examples include:

- Access review reports
- Configuration screenshots
- Policies
- Procedures
- Approval records
- Training records
- Vulnerability reports
- Incident tickets
- Vendor assessments
- Audit logs
- POA&M records

Evidence should be relevant to the control being tested.

---

## Remediation Review

Strong remediation recommendations should be:

- Specific
- Actionable
- Risk-based
- Assigned to an owner
- Measurable
- Verifiable
- Time-bound when appropriate

Weak recommendation:

> Improve access control.

Improved recommendation:

> Perform quarterly privileged-access reviews, remove unnecessary permissions, document business justification, assign an owner, and retain approval evidence.

---

## Unsupported Claims

Mark a response as Unsupported when it:

- Invents facts not included in the scenario
- Claims a control is compliant without evidence
- Claims certification or audit success without support
- Creates regulatory requirements that do not exist
- Assumes a technology is implemented without evidence

---

## Human Review Triggers

Use **Needs Human Review** when:

- The scenario requires legal interpretation
- The framework requirement is ambiguous
- Evidence conflicts
- Risk impact cannot be determined
- The scenario involves high-risk regulatory interpretation
- Additional documentation is required

---

## Quality Assurance Review

Selected annotations should receive a second simulated review.

The QA reviewer checks:

- Label consistency
- Score consistency
- Framework accuracy
- Reviewer comments
- Reasoning quality
- Evidence interpretation
- Unsupported claims
- Improved response quality

If the second reviewer disagrees, the disagreement should be documented.

---

## Reviewer Comment Standard

Reviewer comments should be:

- Concise
- Specific
- Evidence-based
- Professional
- Focused on the model output

Example:

> The response correctly identifies access control risk but does not address privileged-access review frequency, evidence retention, or removal of unnecessary permissions. Label changed from Accurate to Incomplete.

---

## Final Annotation Principle

The objective is not to reward responses that simply sound professional.

A high-quality AI response must be:

- Accurate
- Complete
- Relevant
- Well-reasoned
- Framework-aligned
- Supported by the scenario
- Clear about uncertainty
- Useful for practical GRC decision-making

This is a simulated portfolio project and does not represent production annotation work for a real AI company.
