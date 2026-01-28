# TRANSPARENCY TIERS
## A Balanced Approach to Open Source AI in Government
### The Human Standard

---

## Executive Summary

The Human Standard mandates transparency in government AI systems. However, blanket full transparency creates security vulnerabilities that adversaries can exploit. This document presents a tiered transparency model that preserves accountability while protecting against gaming and exploitation.

**The Core Principle**: Transparency serves accountability. Where full transparency undermines the system's effectiveness, we use alternative accountability mechanisms that achieve the same goal.

---

## Part I: The Tension

### Why Full Transparency Matters

- **Accountability**: Citizens can verify how decisions affecting them are made
- **Bias Detection**: Public scrutiny identifies discriminatory patterns
- **Trust**: Visible systems are trustworthy systems
- **Democratic Control**: Citizens must understand how they're governed

### Why Full Transparency Can Be Problematic

- **Gaming**: Adversaries study the algorithm and optimize to exploit it
- **Security**: Criminal and foreign actors gain operational intelligence
- **Effectiveness**: Some systems only work if their criteria aren't public
- **Privacy**: Fully transparent systems may reveal protected information

### Examples of the Tension

| System | Transparency Benefit | Transparency Risk |
|--------|---------------------|-------------------|
| Tax assessment AI | Ensures fair treatment | Enables evasion optimization |
| Benefits eligibility | Prevents discrimination | Enables fraud optimization |
| Immigration screening | Accountability for denials | Enables visa fraud |
| Fraud detection | Public trust | Criminals avoid detection |
| Border security | Democratic oversight | Adversary exploitation |

---

## Part II: The Tiered Model

### Tier 1: Full Open Source

**Transparency Level**: Code public, weights public, training data disclosed, decision criteria public

**Appropriate For**:
- Routine administrative functions
- Low security risk applications
- High corruption risk areas
- Systems where gaming risk is minimal

**Examples**:
- Permit application processing
- License renewal systems
- Public records requests
- Standard tax calculation (not audit selection)
- Benefits calculation (not fraud detection)
- Court scheduling
- Public comment processing

**Requirements**:
- Full source code published on government repository
- Model weights available for download
- Training data sources disclosed
- Decision explanations provided to affected parties
- Regular third-party audits published

### Tier 2: Audited Closed

**Transparency Level**: Code audited by credentialed third parties; summary and methodology published; decision explanations provided; outcomes publicly reported

**Appropriate For**:
- Moderate security risk applications
- Systems where gaming is possible but not catastrophic
- Areas requiring accountability but also effectiveness

**Examples**:
- Fraud detection systems
- Audit selection criteria
- Immigration initial screening
- Child welfare risk assessment
- Parole recommendation systems
- Loan application screening (government programs)

**Requirements**:
- Source code available to:
  - GAO (Government Accountability Office)
  - Approved academic researchers (with security clearance)
  - Inspector General offices
  - Congressional oversight committees
- Published audit reports (redacted if necessary)
- Aggregate outcome statistics published (by demographic, geography, etc.)
- Individual decision explanations available (redacted criteria if necessary)
- Appeal process with human review

**Audit Requirements**:
- Annual third-party bias audit (published)
- Quarterly accuracy assessment (published)
- Continuous outcome monitoring (dashboard public)

### Tier 3: Classified with Oversight

**Transparency Level**: Closed source; congressional oversight; Inspector General access; aggregate outcomes reported

**Appropriate For**:
- National security applications
- High security risk systems
- Systems where public knowledge would enable serious harm

**Examples**:
- Counterterrorism risk assessment
- Counterintelligence screening
- Sensitive border security systems
- Critical infrastructure threat detection
- Classified information handling

**Requirements**:
- Source code available to:
  - Intelligence committee members (classified briefing)
  - Inspector General (classified access)
  - Cleared oversight staff
- Annual classified audit
- Aggregate statistics reported (classification permitting)
- Appeal process exists (may be classified)
- Five-year sunset requiring reauthorization

**Constraints**:
- Cannot be used for routine law enforcement
- Cannot be used for general population surveillance
- Requires specific authorization for each application
- Subject to FISA-style court review if affecting US persons

---

## Part III: Tier Assignment Criteria

### Decision Framework

```
START
│
├─ Does the system affect individual rights or benefits?
│   ├─ No → Operational system, may be Tier 2 or 3
│   └─ Yes → Continue
│
├─ Would public knowledge enable significant gaming?
│   ├─ No → Tier 1 (Full Open Source)
│   └─ Yes → Continue
│
├─ Would gaming cause serious harm?
│   ├─ No → Tier 1 with monitoring
│   └─ Yes → Continue
│
├─ Is this national security related?
│   ├─ Yes → Tier 3 (Classified with Oversight)
│   └─ No → Tier 2 (Audited Closed)
```

### Tier Assignment Authority

- **Tier 1**: Default for all new systems unless exception granted
- **Tier 2**: Requires agency head approval with written justification
- **Tier 3**: Requires congressional notification and IG review

### Annual Review

All systems classified as Tier 2 or 3 undergo annual review:
- Is the tier classification still justified?
- Have gaming risks changed?
- Are accountability mechanisms working?
- Should transparency increase?

Default direction: Toward greater transparency over time.

---

## Part IV: Accountability Mechanisms by Tier

### Tier 1: Direct Accountability

| Mechanism | Implementation |
|-----------|----------------|
| Public code review | Anyone can examine |
| Academic research | Full access for study |
| Journalism | Full access for investigation |
| Individual challenge | Complete explanation provided |
| Legal discovery | Full disclosure |

### Tier 2: Mediated Accountability

| Mechanism | Implementation |
|-----------|----------------|
| GAO audits | Annual, published with redactions |
| Academic research | Approved researchers with access |
| Journalism | Aggregate data, FOIA for individual cases |
| Individual challenge | Explanation with protected criteria redacted |
| Legal discovery | Court-ordered access with protective order |
| Bias audits | Third-party, published |
| Outcome monitoring | Public dashboard |

### Tier 3: Institutional Accountability

| Mechanism | Implementation |
|-----------|----------------|
| Congressional oversight | Classified briefings |
| Inspector General | Full classified access |
| FISA-style court | Judicial review for sensitive applications |
| Individual challenge | Classified appeal process exists |
| Legal discovery | State secrets privilege applies, but challenge exists |
| Sunset requirement | Must be reauthorized every 5 years |

---

## Part V: Anti-Gaming Measures for Tier 1 Systems

Even fully transparent systems can be hardened against gaming:

### Red Team Requirement

Before any Tier 1 system deploys:
- Professional red team attempts to game it
- Findings addressed before code published
- Red team report published with fixes

### Delayed Publication

- System deploys with 6-month transparency delay
- Period used to identify unexpected vulnerabilities
- Patches developed before code becomes public
- After 6 months, full code published

### Behavioral Monitoring

- All systems include outcome monitoring
- Anomalous patterns trigger investigation
- Rapid response team for identified gaming

### Ensemble Methods

- Use multiple algorithms with non-public weighting
- Individual algorithms are public
- Combination weights are Tier 2 (audited closed)
- Makes gaming significantly harder

### Regular Rotation

- Criteria updated regularly (quarterly)
- Historical criteria published after rotation
- Current criteria may have transparency delay

---

## Part VI: Implementation

### Governance Structure

**AI Transparency Office (ATO)**
- Located within GAO
- Reviews tier classifications
- Conducts Tier 2 audits
- Coordinates with Intelligence Community for Tier 3
- Publishes annual transparency report

**Agency AI Officers**
- Each agency designates AI Transparency Officer
- Responsible for tier classification decisions
- Reports to ATO
- Maintains system inventory

### Classification Process

1. **System Development**: Agency develops AI system
2. **Tier Proposal**: Agency proposes tier classification with justification
3. **ATO Review**: ATO reviews classification (30 days)
4. **Approval/Challenge**: ATO approves or requests modification
5. **Congressional Notification**: Tier 2/3 systems notified to oversight committees
6. **Deployment**: System deployed with appropriate transparency
7. **Annual Review**: Classification reviewed annually

### Transition for Existing Systems

| Timeline | Requirement |
|----------|-------------|
| Year 1 | Inventory all government AI systems |
| Year 2 | Classify all systems by tier |
| Year 3 | Tier 1 systems fully compliant |
| Year 4 | Tier 2 systems fully compliant |
| Year 5 | Tier 3 systems fully compliant |

### Enforcement

- Systems operating without proper tier classification are suspended
- Agency heads personally responsible for compliance
- GAO reports non-compliance to Congress
- Funding can be withheld for non-compliant agencies

---

## Part VII: The Four Principles

Regardless of tier, all government AI systems must satisfy:

### Principle 1: No Black Boxes for Rights Decisions

Any system that affects individual rights, benefits, or liberty must provide:
- An explanation (appropriately redacted if necessary)
- An appeal process with human review
- Outcome data by demographic group

### Principle 2: Democratic Control

All AI systems must:
- Operate within parameters set by elected officials
- Be subject to congressional oversight
- Have sunset provisions requiring reauthorization

### Principle 3: Bias Accountability

All tiers require:
- Regular bias audits (scope depends on tier)
- Published outcome statistics
- Remediation when bias is identified

### Principle 4: Human Override

All tiers require:
- Ability to override any AI decision
- Human review available on request
- Escalation path for contested decisions

---

## Part VIII: Relationship to Fifth Law

The Fifth Law states: "Maintain Transparency—all systems publicly auditable."

**Interpretation**: "Auditable" does not require "fully public." It requires that appropriate oversight bodies can audit and that the public receives sufficient information to hold the system accountable.

Tier 2 and 3 systems satisfy the Fifth Law through:
- Third-party audits (findings published)
- Congressional oversight
- Aggregate outcome transparency
- Individual explanation rights

The spirit of the law—preventing unaccountable black boxes—is preserved while acknowledging that some systems require protected criteria to function.

---

## Part IX: Examples in Detail

### Example 1: Benefits Calculation (Tier 1)

**System**: Social Security benefit amount calculation
**Classification**: Tier 1 (Full Open Source)
**Justification**: Pure calculation, no gaming benefit from knowing formula, high importance of public trust

**Implementation**:
- Full source code on government GitHub
- Training data (anonymized) available
- Decision explanation for every benefit determination
- Public can verify their own calculations

### Example 2: Fraud Detection (Tier 2)

**System**: Benefits fraud detection
**Classification**: Tier 2 (Audited Closed)
**Justification**: Public knowledge of exact criteria would enable fraud optimization

**Implementation**:
- GAO has full access, conducts annual audit
- Academic researchers can access with approval
- Aggregate statistics published (fraud rate by demographic, false positive rate)
- Individuals flagged receive explanation (with criteria redacted) and appeal rights
- Quarterly bias audit published

### Example 3: Counterterrorism Screening (Tier 3)

**System**: International traveler risk assessment
**Classification**: Tier 3 (Classified with Oversight)
**Justification**: National security, adversary exploitation risk

**Implementation**:
- Intelligence committee oversight
- IG has classified access
- FISA court review for US person impacts
- Aggregate statistics (to extent classification permits)
- Redress process exists (may be classified)
- 5-year sunset, reauthorization required

---

## Part X: Objection Responses

### "This is a loophole for secret AI"

**Response**: No. Every system has oversight—the question is who can oversee. Tier 2 systems have GAO, academic, and journalistic access. Tier 3 systems have congressional and IG oversight. The principle of accountability is maintained; only the mechanism varies.

### "Tier 2 and 3 will be abused"

**Response**: Classification requires justification, ATO review, congressional notification, and annual review. The default is Tier 1; agencies must argue for less transparency. Abuse will be caught by oversight mechanisms and annual reviews.

### "This undermines the open source mandate"

**Response**: The mandate's purpose is accountability, not transparency for its own sake. These tiers achieve accountability through different mechanisms. A fully transparent system that can be easily gamed serves no one. An audited system that works serves everyone.

### "Adversaries will still find vulnerabilities"

**Response**: Yes, some gaming will occur. Tier 2 systems are monitored for anomalies. Red teaming before deployment catches many issues. No system is perfect, but tiered transparency is better than either extreme.

---

## Conclusion

Transparency is not binary. Full public transparency serves accountability in most cases, but some systems require protected criteria to function effectively. The tiered model preserves the Human Standard's commitment to accountable AI while acknowledging that one size does not fit all.

The test is not "is everything public?" but "can appropriate oversight bodies audit this system, and does the public have sufficient information to hold it accountable?" Under this framework, the answer is always yes.

---

*"Transparency is a means to accountability, not an end in itself. We achieve accountability through appropriate transparency at every tier."*

—The Human Standard
