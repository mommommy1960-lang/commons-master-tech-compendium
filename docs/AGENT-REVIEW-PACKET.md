# 📘 AGENT REVIEW PACKET

**GitHub + Copilot Engineering Team Standards**  
**For Commons Hardware Validation & Code Review**

---

## PURPOSE

This packet defines the verification standards that all AI agents, automated systems, and human reviewers must apply when evaluating Commons hardware designs, code submissions, and technical documentation.

**Target Audience:**
- GitHub Copilot agents
- Automated CI/CD systems
- Human code reviewers
- Grant review committees
- Safety certification auditors
- External collaborators

---

## VERIFICATION CHECKLIST

Agents must verify the following for EVERY subsystem submission:

###  1. Physical Feasibility

**Requirement:** No subsystem may claim anything beyond documented engineering norms (as of 2025).

**Verification Steps:**
- [ ] All forces, stresses, and loads calculated with safety factors ≥2:1
- [ ] Materials specified with documented properties (yield strength, thermal limits, etc.)
- [ ] No violation of thermodynamic laws (e.g., >100% efficiency, perpetual motion)
- [ ] No claims of superluminal communication, anti-gravity, or energy-from-nothing
- [ ] Dimensions and tolerances achievable with standard manufacturing (CNC, 3D printing, etc.)

**Red Flags:**
- ❌ "Quantum field manipulation"
- ❌ "Zero-point energy harvesting"
- ❌ "Instantaneous matter replication"
- ❌ "Thought-controlled devices" (without documented BCI technology)
- ❌ Claims without citations to peer-reviewed literature

**Approval Criteria:**
- ✅ All claims backed by published research or commercial product specifications
- ✅ Safety factors appropriate for application (2× minimum, 4× for pressure vessels)
- ✅ Materials available from reputable suppliers (McMaster-Carr, Digikey, etc.)

---

### 2. Materials Compliance

**Requirement:** All materials must be real, purchasable, and spec'd with datasheets.

**Verification Steps:**
- [ ] Every material has supplier and part number (or equivalent specification)
- [ ] Material properties documented (tensile strength, thermal conductivity, etc.)
- [ ] Environmental constraints specified (temperature range, humidity, chemical exposure)
- [ ] Availability confirmed (not discontinued or prototype-only)
- [ ] Cost estimates provided (order-of-magnitude accuracy acceptable for R&D)

**Red Flags:**
- ❌ "Unobtainium"
- ❌ "Experimental polymer X-7" (without literature reference)
- ❌ Materials with no supplier information
- ❌ "Military-grade" without specific specification
- ❌ Cost listed as "TBD" or "unknown"

**Approval Criteria:**
- ✅ Every material traceable to commercial source or published synthesis method
- ✅ Material properties within documented ranges for that material class
- ✅ Substitution options provided where possible (e.g., "Lexan 9034 or equivalent polycarbonate")

---

### 3. Test Reproducibility

**Requirement:** Every prototype must define a test that any lab could replicate.

**Verification Steps:**
- [ ] Test procedure written in step-by-step format
- [ ] Required equipment specified with make/model or equivalent spec
- [ ] Pass/fail criteria defined with numerical thresholds
- [ ] Expected results documented (with acceptable tolerance ranges)
- [ ] Safety precautions listed for hazardous tests

**Red Flags:**
- ❌ "Test subjectively for quality"
- ❌ No equipment specifications
- ❌ Pass criteria: "looks good" or "feels right"
- ❌ No safety procedures for high-energy tests
- ❌ Tests requiring equipment not commercially available

**Approval Criteria:**
- ✅ Test procedure follows standard methods (ASTM, ISO, etc.) or clearly documented custom method
- ✅ All measurement equipment specified with accuracy requirements
- ✅ Statistical analysis planned for tests with inherent variability
- ✅ Safety review completed for any test involving pressure, high voltage, high speed, or toxicity

---

### 4. Build Logs

**Requirement:** Commits must link to schematics, BOM, test output, and failure states.

**Verification Steps:**
- [ ] CAD files or text diagrams included (DXF, STL, SVG, or ASCII art)
- [ ] Bill of Materials (BOM) in machine-readable format (CSV, JSON, or Markdown table)
- [ ] Test data logged (CSV, JSON, or database dump)
- [ ] Failure modes documented (if any occurred)
- [ ] Photos or renders of physical build (if prototype exists)

**File Structure Standard:**
```
/system-name/
  ├── README.md (overview, links to other docs)
  ├── schematics/
  │   ├── assembly-diagram.svg
  │   ├── electrical-schematic.pdf
  │   └── cad-model.stl
  ├── bom/
  │   ├── bom.csv (part, qty, source, cost)
  │   └── sourcing-notes.md
  ├── test-results/
  │   ├── test-001-dimensional.csv
  │   ├── test-002-stress.json
  │   └── test-summary.md
  ├── photos/
  │   ├── build-step-01.jpg
  │   └── final-assembly.jpg
  └── failures/
      └── failure-analysis-YYYY-MM-DD.md
```

**Red Flags:**
- ❌ Code-only commits without supporting documentation
- ❌ BOM with missing cost or source information
- ❌ Test results described in prose without raw data
- ❌ No photos of physical hardware
- ❌ Failure states not documented

**Approval Criteria:**
- ✅ Complete documentation set per structure above
- ✅ All files in open formats (prefer SVG over proprietary CAD when possible)
- ✅ QR code assigned and logged in traceability database
- ✅ Git commit message follows format: `[SYSTEM] Brief description (QR: UUID)`

---

### 5. Risk Flags

**Requirement:** Agents must mark unrealistic claims, missing data, safety concerns, under-spec'd power/force loads, and unproven assumptions.

**Categories:**

#### 5.1 Unrealistic Claims
Mark any statement that violates known physics or exceeds documented material capabilities.

**Examples:**
- "Aluminum beam supports 10× its documented yield strength"
- "Battery provides 1000 Wh from 100g cell"
- "Motor produces 10 Nm from 5W input"

**Action:** Flag for review, request citation or correction.

#### 5.2 Missing Data
Mark any specification with TBD, unknown, or incomplete values.

**Examples:**
- "Power consumption: TBD"
- "Material: some kind of plastic"
- "Weight: approximately light"

**Action:** Request specific values with measurement method or calculation.

#### 5.3 Safety Concerns
Mark any design with hazards that lack mitigation.

**High-Priority Hazards:**
- Pressure vessels without relief valves
- High-voltage circuits without isolation
- Rotating machinery without guards
- Toxic materials without ventilation
- Sharp edges on user-contact surfaces
- Thermal hazards (>60°C) without warnings
- Pinch points in automated motion

**Action:** Require safety mitigation or operational restrictions.

#### 5.4 Under-Spec'd Power or Force Loads
Mark any actuator, structure, or power supply that appears undersized.

**Check:**
- Motor torque vs. required load (with safety factor)
- Beam deflection under max load
- Battery capacity vs. power draw (with runtime requirement)
- Bearing load rating vs. applied forces
- Thermal dissipation vs. heat generation

**Action:** Request calculation showing adequacy or upsize component.

#### 5.5 Unproven Assumptions
Mark any claim that assumes behavior without test data or citation.

**Examples:**
- "Self-healing will occur within 1 hour" (without previous test data)
- "Users will find this intuitive" (without usability study)
- "Material will not degrade over time" (without aging test)

**Action:** Request either citation to literature or plan for validation testing.

---

### 6. Evidence Submission

**Requirement:** Attach photos, CAD renders, videos, and sensor logs.

**Evidence Types:**

#### 6.1 Photos
- **Build progress:** At least 5 photos showing assembly stages
- **Final assembly:** Multiple angles, with scale reference (ruler, coin)
- **Detail shots:** Critical components, interfaces, sensors
- **Test setup:** Show test equipment and DUT (device under test)

**Format:** JPG or PNG, minimum 1920×1080, include date stamp in filename

#### 6.2 CAD Renders
- **Exploded view:** Show assembly order and interfaces
- **Section cuts:** Reveal internal structure
- **Dimensioned drawings:** Key measurements with tolerances
- **FEA results:** If structural analysis performed (stress, deflection)

**Format:** PDF (drawings), PNG (renders), STL/STEP (3D models)

#### 6.3 Videos
- **Operation:** Show system in action, normal operation
- **Testing:** Capture test procedure, especially dynamic events
- **Failure modes:** Document any failures for analysis

**Format:** MP4 (H.264), maximum 1080p, include timestamp overlay

#### 6.4 Sensor Logs
- **Raw data:** CSV or JSON format, not processed
- **Metadata:** Sample rate, sensor type, calibration date, units
- **Plots:** Key data visualized (time-series, histograms, etc.)

**Format:** CSV (raw data), PNG (plots), JSON (metadata)

---

## AUTOMATED CHECKS

These checks should be implemented in CI/CD pipeline:

### Code Quality (if software component exists)
```yaml
checks:
  - linter: pylint, eslint, or clang-tidy (language-appropriate)
  - unit_tests: >80% code coverage
  - static_analysis: no critical issues (Coverity, SonarQube)
  - documentation: all public APIs documented
  - license_headers: all files have CERL-1.0 header
```

### Documentation Completeness
```yaml
required_files:
  - README.md (system overview)
  - bom/bom.csv (bill of materials)
  - schematics/*.* (at least one diagram)
  - test-results/*.* (at least one test report)

markdown_checks:
  - no_broken_links: true
  - spell_check: enable (with technical dictionary)
  - format_check: markdownlint rules
```

### BOM Validation
```yaml
bom_columns:
  required: [part_description, quantity, unit_cost, supplier]
  optional: [part_number, datasheet_url, substitute_parts]

bom_checks:
  - no_missing_costs: warn if >10% of line items lack cost
  - no_missing_suppliers: error if any item lacks supplier
  - total_cost_calculated: sum unit_cost × quantity for each line
```

### Test Data Validation
```yaml
test_data_checks:
  - csv_format: valid CSV with header row
  - required_columns: [timestamp, measurement, units, pass_fail]
  - data_range_check: warn if values outside expected range (from spec)
  - statistics_calculated: mean, std_dev, min, max for numeric columns
```

---

## REVIEW WORKFLOW

### Stage 1: Automated Pre-Review (CI/CD)
1. Run automated checks (code quality, doc completeness, BOM validation)
2. Generate review report (list of passes, warnings, errors)
3. Block merge if any errors present
4. Notify author of warnings for manual review

### Stage 2: Agent Review
1. Agent reads submission and cross-references Blue Book specifications
2. Agent verifies physical feasibility (calculations, material properties)
3. Agent checks for risk flags (safety, under-spec, assumptions)
4. Agent generates review comment with line-by-line feedback

**Agent Review Comment Template:**
```markdown
## Agent Review: [System Name] — [Submission ID]

### Summary
- **Status:** [APPROVED / NEEDS REVISION / BLOCKED]
- **Automated Checks:** [X passed, Y warnings, Z errors]
- **Manual Review Items:** [N items require attention]

### Physical Feasibility
- [✅/❌] Forces and loads calculated with appropriate safety factors
- [✅/❌] Materials specified with documented properties
- [✅/❌] No violation of physical laws
- **Comments:** [Detailed feedback if issues found]

### Materials Compliance
- [✅/❌] All materials have supplier/spec information
- [✅/❌] Material properties documented
- [✅/❌] Cost estimates provided
- **Comments:** [Detailed feedback]

### Test Reproducibility
- [✅/❌] Test procedures clearly documented
- [✅/❌] Equipment specified
- [✅/❌] Pass/fail criteria defined
- **Comments:** [Detailed feedback]

### Risk Flags
[List any risks identified, categorized by severity: CRITICAL / HIGH / MEDIUM / LOW]

### Evidence Quality
- Photos: [✅/❌] Adequate coverage
- CAD: [✅/❌] Sufficient detail
- Test Data: [✅/❌] Complete and valid
- **Comments:** [Detailed feedback]

### Recommendations
1. [Action item 1]
2. [Action item 2]
...

### Next Steps
[APPROVED: Ready for merge | NEEDS REVISION: Address items above and resubmit | BLOCKED: Major issues must be resolved]
```

### Stage 3: Human Review (for critical systems)
1. Human reviewer reads agent review and original submission
2. Spot-check calculations and references
3. Assess overall design quality and alignment with Commons mission
4. Provide final approval or request changes

**Systems requiring human review:**
- Pressure vessels (Aurora Mini)
- Personal protective equipment (PFHMS)
- Medical devices (BRL, when applicable)
- Any system with CRITICAL risk flags

---

## ESCALATION PROCEDURES

### Minor Issues (warnings, non-critical gaps)
- **Action:** Agent comments on PR, author addresses in next revision
- **Timeline:** No blocking, but must be resolved before final release

### Major Issues (errors, safety concerns, impossible claims)
- **Action:** Agent blocks merge, requires author response
- **Timeline:** Must be addressed before any further review

### Critical Issues (safety hazards, physics violations)
- **Action:** Agent escalates to human review team, notifies project lead
- **Timeline:** Immediate attention required, may require design re-evaluation

---

## CONTINUOUS IMPROVEMENT

### Agent Training
- Agents should learn from past reviews (false positives, missed issues)
- Quarterly review of agent performance vs. human reviewer findings
- Update agent ruleset based on new standards or technologies

### Standard Updates
- This packet should be reviewed and updated quarterly
- Incorporate lessons learned from build failures and test results
- Align with evolving industry standards (ASTM, ISO updates)

---

## APPENDIX: COMMON FAILURE MODES

### Design Phase
- **Symptom:** Unrealistic performance claims
  - **Cause:** Misunderstanding of material limits or physics
  - **Prevention:** Require citations for all claims beyond established norms

- **Symptom:** Incomplete specifications
  - **Cause:** Rushed design, lack of expertise
  - **Prevention:** Use design checklist, require peer review

### Build Phase
- **Symptom:** Parts don't fit together
  - **Cause:** CAD errors, tolerance stack-up
  - **Prevention:** Tolerance analysis, prototype in cheap material first

- **Symptom:** System doesn't perform as expected
  - **Cause:** Unverified assumptions, modeling errors
  - **Prevention:** Validate sub-systems before integration

### Test Phase
- **Symptom:** Tests fail but system "seems to work"
  - **Cause:** Poorly defined test criteria, measurement errors
  - **Prevention:** Define pass/fail criteria before building, calibrate equipment

- **Symptom:** Inconsistent results
  - **Cause:** Environmental sensitivity, insufficient samples
  - **Prevention:** Control test environment, use statistical analysis

---

## GLOSSARY

**Agent:** Automated system (AI, script, CI/CD tool) that reviews submissions  
**BOM:** Bill of Materials — list of parts required to build system  
**CAD:** Computer-Aided Design — software for creating 3D models  
**CI/CD:** Continuous Integration / Continuous Deployment — automated testing pipeline  
**DUT:** Device Under Test  
**FEA:** Finite Element Analysis — computational structural analysis  
**Red Flag:** Issue that requires immediate attention or blocks approval  
**QR:** Quick Response code — used for traceability in Commons systems  
**TBD:** To Be Determined — placeholder that must be resolved before approval  

---

## DOCUMENT CONTROL

- **Title:** Agent Review Packet
- **Version:** 1.0
- **Date:** 2025-11-14
- **Classification:** Public / Internal Use
- **License:** CERL-1.0 (Commons Ethical Research License)
- **Custodian:** Commons Initiative, Engineering Division
- **Review Cycle:** Quarterly
- **Next Review:** 2026-Q1
- **Status:** ACTIVE

---

## CONTACT

For questions about review standards or to report issues with the review process:

- **Email:** engineering@commonsinitiative.org (fictional example)
- **GitHub:** Open issue in `commons-master-tech-compendium` repository
- **Slack:** #engineering-reviews channel (for Commons team members)

---

*"Review with rigor. Build with confidence. Ship with pride."*
