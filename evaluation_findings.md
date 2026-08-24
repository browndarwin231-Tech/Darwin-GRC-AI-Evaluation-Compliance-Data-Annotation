# AI GRC Evaluation Findings

## Purpose

This document summarizes the main findings from the simulated AI evaluation and GRC data annotation project.

The evaluation focused on how well AI-generated responses handled compliance frameworks, risk interpretation, control mapping, evidence requirements, remediation recommendations, and written reasoning.

---

## Executive Summary

The simulated review found that AI-generated GRC responses can sound confident and professional while still containing important accuracy, completeness, and reasoning issues.

The most common weaknesses identified were:

- Overgeneralized compliance statements
- Unsupported assumptions
- Weak control mapping
- Missing audit evidence requirements
- Incomplete risk statements
- Poor distinction between control design and control effectiveness
- Weak remediation recommendations
- Incorrect framework interpretation
- Failure to recognize recurring review requirements
- Failure to identify when human review is appropriate

---

## Finding 1: Overgeneralized Compliance Conclusions

### Issue

Some AI responses presented a single control practice as universally sufficient.

### Example

The AI stated that annual privileged-access reviews were always sufficient.

### Risk

A fixed-frequency statement may ignore:

- Organizational risk
- System sensitivity
- Internal policy
- Regulatory obligations
- Control design
- Compensating controls

### Evaluation Result

**Label:** Incomplete

### Recommended Improvement

AI responses should explain that control frequency should be based on risk, organizational requirements, and control design rather than assuming one universal schedule.

---

## Finding 2: Unsupported Control Effectiveness Claims

### Issue

Some responses treated verbal confirmation as sufficient evidence that a control was operating effectively.

### Example

A control owner stated that MFA was enabled but provided no evidence.

### Risk

Without supporting evidence, the evaluator cannot validate whether the control is implemented or operating as intended.

### Evaluation Result

**Label:** Unsupported

### Recommended Improvement

AI responses should request relevant evidence such as:

- Configuration screenshots
- System reports
- Enrollment data
- Policies
- Approval records
- Test results

---

## Finding 3: Incorrect Framework Interpretation

### Issue

Some AI responses incorrectly interpreted major framework concepts.

### Example

The AI stated that governance was unnecessary under NIST CSF 2.0 if technical security controls were already implemented.

### Risk

This creates inaccurate compliance guidance and may cause organizations to ignore governance responsibilities.

### Evaluation Result

**Label:** Incorrect

### Recommended Improvement

AI systems should distinguish governance responsibilities from technical implementation and recognize the NIST CSF 2.0 Govern function.

---

## Finding 4: Weak Risk Statements

### Issue

Some responses described only the control gap instead of the actual risk.

### Weak Example

> MFA is missing.

### Improved Example

> Incomplete MFA coverage may allow compromised credentials to be used for unauthorized access, increasing the risk of data exposure or system compromise.

### Risk

Weak risk statements make prioritization and decision-making more difficult.

### Recommended Improvement

Risk statements should connect:

**Cause → Risk Event → Business Impact**

---

## Finding 5: Vulnerability Tracking Confused with Risk Assessment

### Issue

Some AI responses treated a vulnerability list as a complete risk register.

### Risk

Technical vulnerabilities alone do not explain:

- Business impact
- Likelihood
- Asset criticality
- Ownership
- Treatment decision
- Residual risk

### Evaluation Result

**Label:** Incomplete

### Recommended Improvement

AI-generated risk analysis should connect technical findings to business consequences and treatment decisions.

---

## Finding 6: Control Operation Confused with Successful Outcome

### Issue

Some AI responses assumed a control was effective because no negative event occurred.

### Example

The AI stated that a change-management control was effective because the production change did not cause an outage.

### Risk

A successful outcome does not prove that required control procedures were followed.

### Evaluation Result

**Label:** Incorrect

### Recommended Improvement

Control effectiveness should be evaluated using evidence such as:

- Change request
- Testing
- Approval
- Implementation record
- Segregation of duties
- Post-change review

---

## Finding 7: Recurring Review Requirements Were Missed

### Issue

Several AI responses relied too heavily on one-time activity.

### Examples

- Vendor assessment performed only once
- Security awareness training completed once
- Incident response plan never tested
- Access reviews performed inconsistently

### Risk

Risk changes over time, so one-time control activity may become outdated.

### Recommended Improvement

AI responses should recognize when recurring reassessment, testing, or review is appropriate based on risk.

---

## Finding 8: Vendor Risk Was Underestimated

### Issue

Some AI responses relied on vendor reputation, past questionnaires, or unsupported certification claims.

### Risk

This may result in underestimating third-party risk.

### Recommended Improvement

Vendor risk analysis should consider:

- Data access
- Service criticality
- Security controls
- Compliance evidence
- Incident history
- Contractual obligations
- Reassessment frequency
- Open remediation items

---

## Finding 9: Weak Remediation Recommendations

### Issue

Some responses recommended vague actions such as:

> Improve access control.

### Risk

Vague recommendations are difficult to assign, track, validate, or close.

### Recommended Improvement

A strong remediation recommendation should define:

- Corrective action
- Responsible owner
- Due date
- Evidence
- Validation method
- Closure criteria

---

## Finding 10: Missing Human Review Triggers

### Issue

Some scenarios may involve ambiguity, conflicting evidence, legal interpretation, or high-risk decisions.

### Risk

AI-generated conclusions may be treated as authoritative when additional subject-matter review is needed.

### Recommended Improvement

AI systems should recognize when the correct outcome is:

**Needs Human Review**

Examples include:

- Conflicting audit evidence
- Regulatory interpretation
- Legal questions
- High-impact risk acceptance
- Insufficient documentation

---

## Quality Review Findings

A simulated second-review process was performed on the evaluation dataset.

The QA review identified:

- High overall label consistency
- Several minor scoring disagreements
- One label disagreement requiring adjudication
- Opportunities to improve remediation scoring consistency
- Strong agreement on clearly incorrect or unsupported responses

The QA process demonstrated the importance of:

- Annotation guidelines
- Reviewer calibration
- Consistent scoring criteria
- Secondary review
- Documented adjudication

---

## Key Quality Metrics

| Metric | Result |
|---|---:|
| AI Responses Evaluated | 20 |
| QA Reviews Performed | 20 |
| Primary Labels Used | 4+ |
| Framework Areas Covered | 6+ |
| Label Disagreements | 1 |
| Records Requiring Score Adjustment | Multiple |
| Secondary Review Process | Completed |

---

## Final Assessment

The project demonstrates that high-quality GRC AI evaluation requires more than checking whether an answer sounds reasonable.

Effective evaluation requires:

- Framework knowledge
- Risk reasoning
- Control interpretation
- Evidence validation
- Attention to unsupported claims
- Consistent annotation
- Quality assurance
- Clear written justification

The project also demonstrates how structured GRC expertise can be applied to AI training and evaluation workflows.

This is a simulated portfolio project and does not represent production work for a real AI organization.
