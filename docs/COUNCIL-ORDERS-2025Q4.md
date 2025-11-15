# 📘 COUNCIL ORDERS — HARDWARE DIVISION (2025Q4)

**Mandate from the Commons Engineering Council**  
**For All Hardware Development Teams**

---

## PREAMBLE

These orders establish the operational directives for all Commons hardware development from 2025 Q4 forward. They supersede all previous informal guidelines and represent the unified direction of the Engineering Council.

**Authority:** Commons Engineering Council  
**Effective Date:** 2025-11-14  
**Jurisdiction:** All hardware subsystems (Aurora, PFHMS, BRL, CRTS, MPRS, CALEXS)  
**Compliance:** MANDATORY  

---

## ORDER 001 — PUSH ALL SYSTEMS TO MVP PHYSICAL DEMO

**Issued:** 2025-11-14  
**Deadline:** 2026-02-14 (90 days)

### Directive

Within 90 days, each subsystem must produce a physical demonstrator that proves core functionality.

### Requirements by System

**Aurora Mini Centrifuge:**
- [ ] Construct pressure-rated pod (1 atm differential minimum)
- [ ] Install dual-motor rotation system achieving 15–50 RPM
- [ ] Demonstrate radiation shielding with dose measurement
- [ ] Complete vibration analysis at multiple speeds
- [ ] Document all failures and mitigation strategies

**PFHMS v2.0 Tile:**
- [ ] Fabricate 10 tiles with complete layer stack
- [ ] Demonstrate STF stiffening response (<60ms)
- [ ] Test SMA activation under microcontroller control
- [ ] Complete drop-weight testing (5kg, 2m minimum)
- [ ] Validate electronics (IMU logging, battery life >8hr)

**BRL Soft-Limb Segment:**
- [ ] Create single 300mm segment with self-healing skin
- [ ] Demonstrate conductivity recovery after 5mm cut
- [ ] Achieve 90° flexion with cable actuation system
- [ ] Map sensor response to bend angle (calibration curve)
- [ ] Complete 1,000 flex cycle durability test

**CRTS Multi-Material Fabrication Cell:**
- [ ] Build CoreXY gantry with 400×400mm workspace
- [ ] Install 4-material toolhead carousel
- [ ] Demonstrate successful printing with each material
- [ ] Implement QR traceability with database logging
- [ ] Complete 24-hour continuous operation test

**MPRS Navigation Robot:**
- [ ] Assemble mobile platform with LIDAR and RGB-D camera
- [ ] Implement SLAM navigation (ROS-based)
- [ ] Map 500m² test area with <5cm accuracy
- [ ] Demonstrate autonomous waypoint navigation
- [ ] Test auto-docking with >90% success rate

**CALEXS XR Pod:**
- [ ] Install 3-screen immersive display system
- [ ] Deploy haptic floor with 12-zone control
- [ ] Integrate XR headset with biometric monitoring
- [ ] Create 3 demo experiences (education, therapy, entertainment)
- [ ] Complete user comfort study (10 participants, 30min each)

### Success Criteria

A system is considered **MVP Complete** when:
1. Physical hardware demonstrates core functionality
2. All safety systems operational (e-stops, interlocks, guards)
3. Test data logged and reviewed (pass/fail per Blue Book standards)
4. Build documentation complete (photos, BOM, schematics)
5. QR traceability assigned and database updated
6. Failure modes documented with mitigation plans

### Consequences of Non-Compliance

- Systems not reaching MVP within 90 days will be flagged for priority review
- Resources may be reallocated to systems on track
- Project leads must provide weekly status updates if behind schedule

---

## ORDER 002 — NO SPECULATIVE PHYSICS

**Issued:** 2025-11-14  
**Status:** PERMANENT

### Directive

Any attempt to bypass physical laws is forbidden in all Commons designs.

### Prohibited Claims

The following are **BANNED** from all designs, documentation, and demonstrations:

❌ **Anti-gravity or gravity manipulation** (beyond centripetal force)  
❌ **Faster-than-light communication or travel**  
❌ **Perpetual motion or over-unity energy devices**  
❌ **Cold fusion or zero-point energy extraction**  
❌ **Teleportation of matter**  
❌ **Time travel or causality violation**  
❌ **Consciousness upload or mind-reading** (without documented BCI technology)  
❌ **Instantaneous fabrication** (all processes require realistic time)  
❌ **Biological immortality or instant regeneration**  
❌ **Force fields or energy shields** (physical barriers only)  

### Allowed Technologies

The following are **APPROVED** as they align with established physics:

✅ **Centrifugal artificial gravity** (rotational acceleration)  
✅ **Radiation shielding** (mass-based attenuation: HDPE, tungsten, lead)  
✅ **Self-healing materials** (chemical re-bonding, documented in literature)  
✅ **Shape-memory alloys** (thermally or electrically activated, e.g., Nitinol)  
✅ **Additive manufacturing** (3D printing, multi-material extrusion)  
✅ **Autonomous robotics** (SLAM, computer vision, path planning)  
✅ **Immersive XR** (headsets, haptics, multi-sensory integration)  
✅ **Soft robotics** (compliant actuators, flexible materials)  

### Verification Process

Before ANY new technology concept is added to a Commons system:
1. Author must provide **peer-reviewed citation** demonstrating feasibility
2. Engineering Council reviews citation for credibility
3. If approved, technology added to "Allowed Technologies" list
4. If rejected, author must revise or abandon concept

### Consequences of Violation

- First violation: Formal warning, revision required
- Second violation: Author removed from project
- Deliberate violation: Immediate project termination, author banned from Commons contributions

---

## ORDER 003 — TRACEABILITY MANDATE

**Issued:** 2025-11-14  
**Status:** PERMANENT

### Directive

All fabrication, sensor logs, and trials must be QR-traceable.

### Requirements

Every physical component, assembly, and test must have:
1. **Unique QR code** (UUID format, e.g., `550e8400-e29b-41d4-a716-446655440000`)
2. **Database entry** linking QR to build/test data
3. **Permanent marking** (laser etched, printed label, or stamped)

### QR Code Standard

**Format:** QR Code, Version 2 (25×25 modules), Error Correction Level M (15%)  
**Data:** UUID (36 characters)  
**Size:** Minimum 10mm × 10mm for reliable scanning  
**Placement:** Visible location, does not interfere with function  

**Example QR Payload:**
```
https://commons.db/trace/550e8400-e29b-41d4-a716-446655440000
```

### Database Schema (Minimum Required Fields)

```json
{
  "uuid": "550e8400-e29b-41d4-a716-446655440000",
  "system": "PFHMS",
  "component": "Smart Armor Tile #47",
  "build_date": "2025-11-14T18:30:00Z",
  "operator": "user_id_42",
  "machine": "crts_cell_01",
  "materials": [
    {"name": "Kevlar fabric", "batch": "KEV-2025-10-B3"},
    {"name": "STF gel", "batch": "STF-2025-11-A1"},
    {"name": "Nitinol wire", "batch": "NIT-2025-09-C2"}
  ],
  "parameters": {
    "layer_thickness": "1.2mm",
    "cure_time": "300s",
    "temperature": "23C"
  },
  "tests": [
    {
      "test_id": "TEST-001",
      "test_type": "drop_weight",
      "result": "PASS",
      "measurement": "Peak force: 1250N (spec: <1500N)"
    }
  ],
  "photos": [
    "https://commons.storage/photos/tile-47-front.jpg",
    "https://commons.storage/photos/tile-47-back.jpg"
  ]
}
```

### Scanning and Retrieval

- All QR codes must be scannable with standard smartphone camera apps
- Database must be accessible via web interface and REST API
- Search capability by UUID, date range, system type, operator, test result

### Consequences of Non-Compliance

- Components without QR codes are considered **untraceable** and cannot be used in production or testing
- Undocumented builds must be scrapped and rebuilt
- Persistent non-compliance: Project on hold until traceability established

---

## ORDER 004 — SAFETY PROTOCOLS

**Issued:** 2025-11-14  
**Status:** PERMANENT

### Directive

All pressure-vessel and high-RPM tests require shielding, remote activation, and fail-stop sensors.

### Tier 1 Hazards (Mandatory Protection)

**Pressure Vessels** (Aurora Mini, CRTS heated bed, any pressurized component)
- [ ] Design per ASME BPVC with 4:1 safety factor minimum
- [ ] Pressure relief valve (automatic, set at 1.5× working pressure)
- [ ] Blast shield (polycarbonate or steel, rated for 2× stored energy)
- [ ] Remote pressure monitoring with auto-shutoff at 1.3× working pressure
- [ ] Operator distance ≥3m during pressurization

**High-Speed Rotation** (Aurora Mini centrifuge, CRTS spindle)
- [ ] Containment shield rated for 2× max RPM failure speed
- [ ] Vibration sensor with automatic shutdown (threshold: 2× normal operation)
- [ ] Imbalance detection (accelerometer-based, shutdown if >1mm/s RMS)
- [ ] Mechanical brake (fail-safe, engages on power loss)
- [ ] Operator distance ≥2m during operation

**High Voltage** (>50V DC or >30V AC)
- [ ] Insulation rated for 2× operating voltage
- [ ] GFCI protection on all AC circuits
- [ ] Warning labels on enclosures
- [ ] Lockout/tagout procedures for maintenance
- [ ] Operator training on electrical safety

### Tier 2 Hazards (Standard Protection)

**Thermal** (hotends, heated beds, >60°C surfaces)
- [ ] Thermal runaway protection in firmware
- [ ] Temperature monitoring with auto-shutoff (>10% over setpoint)
- [ ] Guarding or warning labels on hot surfaces
- [ ] Heat-resistant enclosure materials

**Mechanical Motion** (robots, gantries, actuators)
- [ ] Emergency stop buttons (large, red, accessible from all positions)
- [ ] Force limiting (software or mechanical, <50N pinch force)
- [ ] Proximity sensors in pinch-point areas
- [ ] Motion interlocks (stop if enclosure opened)

**Chemical** (batteries, STF gel, self-healing polymers)
- [ ] Material Safety Data Sheets (MSDS) on file
- [ ] Proper ventilation (fume hood or outdoor use if required)
- [ ] Personal protective equipment (gloves, goggles as specified in MSDS)
- [ ] Spill containment and cleanup materials on hand

### Testing Safety Checklist

Before ANY high-energy test (pressure, rotation, impact, electrical):
- [ ] Safety plan written and approved
- [ ] All personnel briefed on hazards and emergency procedures
- [ ] Test area cleared of non-essential personnel
- [ ] Shielding in place and verified
- [ ] Remote activation system tested
- [ ] Emergency stop tested
- [ ] First aid kit and fire extinguisher accessible
- [ ] Communication plan (radio, phone) established

### Incident Reporting

Any safety incident (near-miss, minor injury, property damage) must be:
1. Reported within 24 hours to Engineering Council
2. Documented in incident report (form available in `/governance/safety/`)
3. Root cause analysis completed within 7 days
4. Corrective actions implemented before testing resumes

Serious incidents (major injury, significant property damage) require:
1. Immediate work stoppage
2. Notification to project lead and safety officer
3. External safety audit before work resumes

---

## ORDER 005 — INTERSUBSYSTEM COORDINATION

**Issued:** 2025-11-14  
**Status:** ONGOING

### Directive

Aurora Mini integrates with PFHMS (crew safety), CRTS (module fabrication), and CALEXS (training module).

### Integration Milestones

**Phase 1: Interface Specification (Complete by 2025-12-14)**
- [ ] Define physical mounting interfaces between systems
- [ ] Specify electrical interfaces (power, data, control signals)
- [ ] Document communication protocols (UART, I2C, WiFi, etc.)
- [ ] Create integration test plan

**Phase 2: Subsystem Integration (Complete by 2026-02-14)**
- [ ] Aurora Mini + PFHMS: Test radiation shielding effectiveness on PFHMS tiles
- [ ] Aurora Mini + CRTS: Fabricate Aurora components (gaskets, mounting brackets) on CRTS cell
- [ ] Aurora Mini + CALEXS: Create VR training module for Aurora operation
- [ ] MPRS + CRTS: Robot delivers materials to fabrication cell, retrieves finished parts
- [ ] CALEXS + BRL: VR rehabilitation exercises with BRL limb haptic feedback

**Phase 3: Full System Demo (Complete by 2026-05-14)**
- [ ] Demonstrate complete workflow: Design in CALEXS → Fabricate on CRTS → Deliver via MPRS → Install on Aurora
- [ ] Public demonstration event (Commons Hardware Lab opening)
- [ ] Documentation: Video, photos, technical report

### Coordination Meetings

- **Frequency:** Bi-weekly (every other Wednesday, 10:00 AM Pacific)
- **Attendance:** Lead engineer from each subsystem (mandatory)
- **Agenda:** Integration status, blockers, upcoming milestones
- **Minutes:** Published to `/docs/integration-meetings/` within 48 hours

---

## ORDER 006 — EXPANSION PREP

**Issued:** 2025-11-14  
**Deadline:** Ongoing, with key milestones

### Directive

Teams prepare scale-up plans for Seattle Pilot Lab, XR Learning Suite, and Commons Public Demonstrator Unit.

### Seattle Pilot Lab (Target: 2026-Q2)

**Facility Requirements:**
- 500–1000 m² warehouse or industrial space
- 200A electrical service (3-phase preferred)
- HVAC for climate control (18–25°C)
- Loading dock for equipment delivery
- Office space for 5–10 staff
- Conference room for demonstrations and training

**Equipment to Deploy:**
- 1× Aurora Mini (full testbed with observation platform)
- 100× PFHMS tiles (demonstration vest + spares)
- 2× BRL limb segments (research station)
- 1× CRTS fabrication cell (operational, 24/7 capable)
- 3× MPRS navigation robots (fleet coordination demo)
- 2× CALEXS XR pods (public access, educational programs)

**Programs:**
- Public demo days (monthly, free admission)
- School field trips (K–12, aligned with STEM curriculum)
- Maker workshops (weekend sessions, hands-on projects)
- Research partnerships (university co-labs, internships)

**Funding Target:** $500K–$1M (equipment, facility, first-year operations)

---

### XR Learning Suite (Target: 2026-Q3)

**Concept:** Network of CALEXS pods in educational institutions

**Deployment Sites (Phase 1):**
- Seattle Central College (community college)
- University of Washington (research university)
- Garfield High School (public high school)
- Seattle Public Library (Central branch)

**Content Development:**
- 20+ educational experiences (STEM subjects, history, arts)
- 10+ therapy/wellness programs (anxiety management, PTSD treatment)
- 5+ professional training modules (crisis response, public speaking)

**Technical Requirements:**
- Network linking (low-latency, shared experiences)
- Content management system (centralized distribution)
- User analytics (learning outcomes, engagement metrics, privacy-compliant)

**Funding Target:** $250K–$500K (pod deployment, content development, first-year support)

---

### Commons Public Demonstrator Unit (Target: 2026-Q4)

**Concept:** Mobile demonstration unit (trailer or van) for outreach

**Equipment:**
- Scaled-down Aurora Mini (tabletop demo, 0.5m diameter)
- PFHMS tile samples (hands-on, visitors can feel stiffening response)
- BRL limb segment (demonstration, not user-controlled)
- CRTS cell live demo (print on-demand souvenirs, QR-traced)
- MPRS robot (interactive, visitors can send commands)
- CALEXS "pod lite" (single-screen XR, 5-minute experiences)

**Tour Schedule:**
- Seattle: 10 events (community centers, schools, festivals)
- Regional: 5 cities (Portland, Vancouver BC, Spokane, Boise, San Francisco)
- National: 2 conferences (Maker Faire, ISTE, or equivalent)

**Staffing:**
- 2 full-time demo specialists
- Volunteer support (trained Commons ambassadors)

**Funding Target:** $150K–$300K (vehicle conversion, equipment, first-year operations)

---

### Scale-Up Planning Deliverables (by 2026-01-14)

Each subsystem team must provide:
- [ ] **Cost model:** Price per unit at production scale (10, 100, 1000 units)
- [ ] **Supply chain:** Identify critical components, lead times, alternative suppliers
- [ ] **Manufacturing plan:** Make vs buy analysis, contract manufacturing options
- [ ] **Support model:** Maintenance, consumables, training requirements
- [ ] **Expansion timeline:** 6, 12, 24-month roadmap for scaling

---

## ORDER 007 — DOCUMENTATION STANDARD

**Issued:** 2025-11-14  
**Status:** PERMANENT (addendum to existing orders)

### Directive

All technical documentation must follow Commons Markdown Standard.

### File Format Standards

**Primary:** Markdown (.md) for all technical documentation  
**Secondary:** PDF (for archival), CSV (for tabular data), JSON (for structured data)  
**CAD/Graphics:** SVG (preferred), PNG (raster), STL/STEP (3D models)

### Markdown Style Guide

**Headings:**
```markdown
# System Name (H1, document title only)
## Major Section (H2)
### Subsection (H3)
#### Detail (H4, use sparingly)
```

**Code Blocks:**
- Use fenced code blocks with language identifier
- For ASCII art diagrams, use ` ```text ` or ` ``` ` (no language)

**Tables:**
- Use Markdown tables with header row
- Align columns with pipes for readability
- Include units in column headers

**Links:**
- Use relative links for internal documents: `[Blue Book](../docs/COMMONS-BLUE-BOOK.md)`
- Use absolute URLs for external references
- Check all links before committing (no broken links)

**Images:**
- Store in `/photos/` or `/schematics/` subdirectory
- Use descriptive filenames: `aurora-mini-side-view.png`
- Include alt text: `![Aurora Mini side view](photos/aurora-mini-side-view.png)`

### Document Structure Template

```markdown
# [System Name] — [Document Type]

**Version:** X.Y  
**Date:** YYYY-MM-DD  
**Status:** [Draft | Review | Approved]  
**Author:** [Name or Team]  

---

## Overview
[Brief description of the system/document purpose]

## [Major Section 1]
[Content]

## [Major Section 2]
[Content]

## References
1. [Citation 1]
2. [Citation 2]

---

**Document ID:** [Unique identifier]  
**License:** CERL-1.0  
**Next Review:** [Date]
```

---

## ORDER 008 — QUARTERLY REVIEW MANDATE

**Issued:** 2025-11-14  
**Status:** PERMANENT

### Directive

All systems undergo quarterly engineering review with documented assessment.

### Review Schedule

- **Q1 Review:** January 15, 2026
- **Q2 Review:** April 15, 2026
- **Q3 Review:** July 15, 2026
- **Q4 Review:** October 15, 2026

### Review Agenda (3 hours per system)

1. **Status Report** (30 min)
   - Progress since last review
   - Milestones achieved vs. planned
   - Current blockers and mitigation plans

2. **Technical Deep Dive** (60 min)
   - Demonstration of working prototype
   - Test results review (successes and failures)
   - Design changes and rationale

3. **Safety & Compliance** (30 min)
   - Safety incidents since last review
   - Compliance status (standards, certifications)
   - Risk assessment updates

4. **Integration & Collaboration** (30 min)
   - Inter-system coordination status
   - External partnerships
   - Resource sharing opportunities

5. **Planning & Resources** (30 min)
   - Next quarter milestones
   - Resource needs (budget, personnel, equipment)
   - Grant applications and funding status

### Review Panel

- Commons Engineering Council (3 members)
- External advisor (relevant expertise)
- Safety officer
- Documentation lead

### Review Outcomes

Each system receives rating:
- **Green:** On track, no significant issues
- **Yellow:** Minor concerns, corrective actions planned
- **Red:** Major issues, requires intervention

Rating determines:
- Resource allocation for next quarter
- Frequency of check-ins (green: quarterly, yellow: monthly, red: weekly)
- Escalation to leadership if red for 2 consecutive quarters

---

## ORDER 009 — OPEN SOURCE COMMITMENT

**Issued:** 2025-11-14  
**Status:** PERMANENT

### Directive

All Commons hardware designs released under CERL-1.0 license with full documentation.

### License Requirements

**Hardware Designs:**
- License: CERN Open Hardware License v2.0 (Strongly Reciprocal variant) OR CERL-1.0
- Include: LICENSE file in repository root
- Header: All design files include license header comment

**Software:**
- License: MIT OR Apache 2.0 (permissive), GPL v3 (copyleft), or CERL-1.0
- Include: LICENSE file, NOTICE file (if Apache 2.0)
- Header: All source files include license header

**Documentation:**
- License: Creative Commons BY-SA 4.0 OR CERL-1.0
- Include: License footer on all markdown documents

### Release Checklist

Before public release of any subsystem:
- [ ] All files have appropriate license headers
- [ ] README includes build instructions
- [ ] BOM included with sourcing information
- [ ] Safety warnings prominently displayed
- [ ] Known issues documented
- [ ] Contributing guidelines provided (CONTRIBUTING.md)

### Exclusions from Open Source

The following may be kept proprietary (if necessary for commercial viability):
- Manufacturing process details (beyond what's needed to replicate)
- Supplier pricing agreements
- Customer lists or deployment locations
- Security-sensitive configurations

However, preference is for full open source whenever possible.

---

## ORDER 010 — ETHICS & MISSION ALIGNMENT

**Issued:** 2025-11-14  
**Status:** PERMANENT

### Directive

All Commons technologies must advance ethical, non-coercive, human-sovereignty-preserving goals.

### Prohibited Applications

Commons hardware may NOT be used for:
- ❌ Weapons or military offensive systems
- ❌ Surveillance or tracking without informed consent
- ❌ Manipulation or coercion of individuals
- ❌ Environmental harm or resource exploitation
- ❌ Discrimination or exclusion based on protected characteristics

### Required Considerations

Before ANY new feature or application:
- [ ] Dual-use analysis (could this be weaponized or abused?)
- [ ] Privacy impact assessment (what data is collected, who has access?)
- [ ] Accessibility evaluation (can this be used by people with disabilities?)
- [ ] Environmental impact (energy use, materials, waste)
- [ ] Equity analysis (does this benefit or harm marginalized communities?)

### Approval Process for Sensitive Applications

If a proposed use case raises ethical concerns:
1. Submit to Ethics Review Board (3-member panel)
2. Provide detailed use case description and risk mitigation
3. Board reviews within 14 days (approve, deny, or request modifications)
4. Decision is binding; appeals go to Engineering Council

### Example Case Studies

**Approved:**
- PFHMS tiles for firefighter protection (safety)
- CALEXS for PTSD therapy (consent-based, therapeutic)
- MPRS for hospital delivery (service, non-coercive)

**Denied:**
- PFHMS for riot police (potential for abuse)
- CALEXS for interrogation training (coercive)
- MPRS with facial recognition for public spaces (surveillance)

**Conditional Approval:**
- BRL for military prosthetics (approved only for medical rehabilitation, not enhancement for combat)

---

## ENFORCEMENT & ACCOUNTABILITY

### Compliance Monitoring

- **Quarterly audits:** Random selection of 25% of active projects
- **Anonymous reporting:** Hotline for ethics or safety concerns
- **Transparent documentation:** All council orders published publicly

### Penalties for Non-Compliance

**Minor violations** (unintentional, first offense):
- Written warning
- Corrective action plan (1 week to comply)
- Additional oversight for 1 quarter

**Major violations** (reckless disregard for safety, ethics, or physics):
- Project suspension
- Team lead removed
- Independent review before reinstatement

**Severe violations** (deliberate falsification, dangerous conduct):
- Project termination
- Contributors banned from Commons
- Public disclosure of violation (for safety)

---

## AMENDMENT PROCESS

Council Orders may be amended by:
1. Proposal from any Engineering Council member
2. Review by full council (7-day comment period)
3. Vote: 2/3 majority required for approval
4. Publication: Amended order published within 24 hours
5. Effective date: 30 days after publication (unless emergency)

---

## CONCLUSION

These orders establish the foundation for rigorous, ethical, safe, and collaborative hardware development in the Commons Initiative.

**Remember:**
- **Safety first:** Protect people, protect equipment, protect reputation
- **Reality-based:** Physics doesn't negotiate
- **Traceable:** Every component, every test, every decision
- **Open:** Share knowledge, collaborate, lift others up
- **Ethical:** Build for humanity, not against it

---

**Document Control**
- **Title:** Council Orders — Hardware Division (2025Q4)
- **Version:** 1.0
- **Issued:** 2025-11-14
- **Authority:** Commons Engineering Council
- **Classification:** Public / Internal
- **License:** CERL-1.0
- **Next Review:** 2026-01-15 (quarterly cycle)
- **Status:** ACTIVE — Enforceable immediately

---

*"Build the future. Respect the present. Honor the past."*
