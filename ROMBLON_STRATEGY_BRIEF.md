# Romblon Smart Province Initiative
## Strategic Brief v1.0

**Lead Proponent:** Climate Smart Ventures (CSV)  
**Technology Partner:** Likha Labs  
**Date:** January 2026  
**Status:** Unsolicited Proposal — Concept Stage

---

## Executive Summary

The **Romblon Smart Province Initiative** is a dual-track pilot program to demonstrate how AI-powered governance and EdTech can transform small island provinces with limited resources. CSV and Likha Labs propose an unsolicited PPP for AI governance services, combined with national agency partnerships (DICT/DepEd) for EdTech deployment.

**Why Romblon?**
- 302,824 population across 17 municipalities (3 major islands)
- Small enough to pilot affordably; big enough to prove national scalability
- Island geography mirrors 463 other Philippine municipalities
- Limited LGU staff (3-5 per office) = high AI force-multiplier impact
- Strong economic base (marble industry, tourism) for workforce development alignment

**Core Offering:**
1. **LGU AI Platform** — 24/7 citizen helpdesk, business permit automation, budget intelligence, public advisory system
2. **EdTech Ecosystem** — AI learning platform, skills training (tourism/marble/BPO), teacher development, jobs pathway tracker

**Investment:** ₱12M CSV (AI governance) + ₱18M grants (EdTech) = ₱30M total  
**Timeline:** 6-month pilot → 17-municipality rollout by Month 12  
**ROI for Romblon:** 70% faster permits, ₱8M/year savings, 3x business registrations, 25% reduction in youth out-migration

---

## 1. Market Context & Opportunity

### The Challenge: Island Governance at Breaking Point

Romblon's 17 municipalities face the same service delivery pressures as Metro Manila—with 10% of the resources:

- **8-hour wait times** for simple permits/inquiries (staff stretched across offices)
- **68% youth out-migration** post-graduation (skills mismatch, limited opportunities)
- **Zero digital tools** for LGU operations (paper-based processes, manual routing, no analytics)
- **EODB compliance gap**: RA 11032 mandates 3-day simple permits, 20-day complex permits—impossible without automation

### Why Now: Regulatory Tailwinds

- **RA 11032 (EODB, 2018)** — Mandates digital processing for permit timelines
- **RA 11055 (PSED, 2018)** — Free tertiary education demands quality EdTech infrastructure
- **RA 10929 (Free Internet, 2017)** — Public WiFi enables last-mile digital services
- **DepEd Digital Transformation Roadmap 2023–2028** — National push for AI/digital learning tools
- **DICT Cloud First Policy (2020)** — Mandates cloud adoption for government systems

### The Opportunity: National Pilot to 1,488 LGUs

If successful, Romblon becomes the **reference model** for:
- **463 island municipalities** with similar geography/constraints
- **50+ island provinces** (2M+ citizens) by 2028
- **DICT eGov PH System** validation at provincial/municipal scale
- **DepEd AI integration** blueprint for 47,000+ public schools nationwide

---

## 2. Solution Architecture

### System 1: LGU AI Platform (Governance)

Built on **Accord Platform** (Likha Labs IP) — governance-by-design OS with audit trails, RBAC, DPIA-compliant, Cloud First aligned.

**Core Features:**
1. **24/7 AI Citizen Helpdesk**
   - Natural language interface (Tagalog + Romblomanon)
   - Answers inquiries on permits, services, requirements, schedules
   - SMS/web/Facebook Messenger integration
   - Escalation to human staff for complex cases

2. **Business Permit Automation (EODB Compliance)**
   - Digital application + document upload
   - Automated routing to approving offices
   - Real-time status tracking for applicants
   - Compliance checks against RA 11032 timelines
   - Payment integration (GCash, PayMaya, online banking)

3. **Budget & Procurement Intelligence**
   - AI analysis of budget utilization (variance alerts)
   - Procurement anomaly detection (price benchmarking, duplicates)
   - COA audit readiness dashboards
   - Multi-year trend visualization

4. **Public Advisory System**
   - Disaster alerts (typhoon, flood, earthquake)
   - Health advisories (dengue outbreaks, vaccination campaigns)
   - Program announcements (scholarships, livelihood, social services)
   - Multi-channel broadcast (SMS, social media, municipal websites)

5. **Cross-Municipality Data Sharing**
   - Shared constituent database (birth certificates, business records)
   - Inter-LGU permit endorsements (e.g., Romblon → Odiongan transfer)
   - Provincial dashboards for governor oversight

**Technical Stack:**
- Backend: NestJS + TypeScript + Prisma (PostgreSQL) + Redis (BullMQ)
- Frontend: Next.js 14 + React 19 + Tailwind + Radix UI
- AI: OpenAI GPT-4o (multilingual NLP), custom fine-tuning for Romblomanon/Onhan/Asi
- Infrastructure: AWS/GCP (DICT Cloud First compliant), 99.5% uptime SLA

### System 2: EdTech Ecosystem (Education)

**Core Features:**
1. **AI-Powered Learning Platform**
   - Adaptive learning paths (adjusts to student pace/level)
   - Multilingual content (Tagalog, English, Romblomanon)
   - Gamified modules for K-12 subjects
   - AI tutoring for struggling learners (math, science, reading)

2. **Skills Training: Tourism, Marble Industry, BPO-Ready**
   - Tourism: Hospitality, tour guiding, customer service
   - Marble: Stonework techniques, quality control, export standards
   - BPO: English proficiency, typing, virtual collaboration tools
   - Micro-credentials + digital badges (shareable on LinkedIn)

3. **Teacher Professional Development**
   - Digital pedagogy training (blended learning, flipped classroom)
   - AI tools for lesson planning + assessment automation
   - Community of practice (province-wide teacher network)
   - DepEd INSET credit-eligible modules

4. **Jobs Pathway Tracker**
   - Skills inventory matched to local job openings (tourism, marble, retail)
   - Remote work opportunities (BPO, freelancing, gig economy)
   - Employer partnerships (AC Energy, marble exporters, resorts)
   - Post-graduation placement tracking

5. **Romblon State University Integration**
   - Unified student records (high school → university transition)
   - Dual-enrollment programs (technical skills + academic credit)
   - Research collaboration (RSU students as platform testers/improvers)

**Technical Stack:**
- Learning Management: Moodle + custom AI layer (OpenAI fine-tuned models)
- Student Information System: Integration with DepEd LIS (Learner Information System)
- Content Delivery: CDN for video/interactive modules (low-bandwidth optimized)
- Analytics: Student progress dashboards for teachers, division office, DepEd

---

## 3. Personas & Impact

### Mayor Juan — Municipal Mayor, Town of Odiongan
**Pain Points:**
- Buried in paper reports; no real-time visibility into budget burn rate
- COA audit observations on procurement irregularities (delayed bidding)
- Citizen complaints about slow permit processing hurt re-election prospects

**How Platform Helps:**
- Real-time budget dashboard (₱X spent vs allocated, by office/program)
- AI flags procurement anomalies 30 days before COA review (time to fix)
- EODB compliance dashboard shows 3-day permit target vs actual (transparency)

**Impact Metrics:**
- 60% faster decision-making (data at fingertips, not buried in Excel)
- Zero audit observations on AI-flagged items (proactive compliance)
- Citizen satisfaction (NPS) improves from 42 → 68 in 6 months

### Teacher Maria — Grade 6 Teacher, Romblon Central School
**Pain Points:**
- 45 students per class; 12 are 2 grade levels behind in reading
- No time for individualized tutoring (4 sections to teach daily)
- Limited digital resources (1 laptop, unreliable internet)

**How Platform Helps:**
- AI tutor gives struggling students personalized reading exercises (adaptive)
- Automated grading for quizzes (saves 5 hours/week, reallocates to 1-on-1 time)
- Offline-capable mobile app (students practice at home without WiFi)

**Impact Metrics:**
- 40% improvement in student engagement (gamified modules motivate learners)
- 25% reduction in dropout rates (struggling students get AI-powered safety net)
- Teacher satisfaction (NPS) improves from 55 → 72

### Entrepreneur Carlo — Marble Workshop Owner, San Jose
**Pain Points:**
- Business permit renewal takes 21 days (loses contracts due to delay)
- Can't find skilled marble workers (youth migrate to Manila)
- No access to government support programs (unaware of DOST grants)

**How Platform Helps:**
- Digital permit renewal in 3 days (EODB compliance, online payment)
- Trains 5 new hires via marble skills modules (micro-credentials recognized by buyers)
- AI helpdesk alerts him to DOST P500K equipment grant (matches his profile)

**Impact Metrics:**
- 3-day permit processing (vs 21 days baseline) = faster contract turnaround
- 5 new hires trained via platform = 30% workforce expansion
- ₱500K grant secured (AI-flagged opportunity) = new CNC marble cutter purchased

---

## 4. Partnership Model & Pricing

### Track 1: LGU PPP (Unsolicited Proposal)

**Structure:** Build-Operate-Transfer (BOT) • 3-year concession

**CSV Investment:** ₱12M upfront
- Platform deployment + customization: ₱5M
- Training (LGU staff, barangay officials): ₱2M
- Infrastructure (servers, bandwidth, devices): ₱3M
- Operations (Year 1-3 support): ₱2M

**LGU Payment:** ₱150K/month per municipality (~₱2.5M/year provincial-wide)
- 17 municipalities × ₱150K = ₱2.55M/month (₱30.6M/year)
- Provincial government pays on behalf of municipalities (bulk pricing discount)

**Revenue Share:** 70% CSV, 30% Romblon Provincial Government
- CSV: ₱21.4M/year (70% of ₱30.6M)
- Province: ₱9.2M/year (reinvested in digital infrastructure: fiber, devices, public WiFi)

**Transfer:** Full IP and operations transfer to province after Year 3
- CSV trains provincial IT staff to maintain platform
- Source code, documentation, admin credentials transferred
- Optional: ₱500K/year maintenance contract (Years 4-10) for updates/support

**Legal Framework:**
- RA 11966 (PPP Code) Sec 10: Unsolicited proposal procedures
- RA 12009 (Procurement Act) Sec 22: E-procurement, audit trails
- RA 10173 (Data Privacy Act) Sec 11(d), Sec 20: Data residency, DPIA
- DICT Cloud First Policy (2020): Cloud infrastructure compliance

### Track 2: National Agency Partnership (EdTech)

**Structure:** Grant-funded pilot + LGU co-funding

**Funding Sources:**
- DICT ICT Office: ₱8M (digital infrastructure grant)
- DepEd Digital Transformation Fund: ₱6M (learning platform deployment)
- DOST-PCIEERD: ₱4M (skills training modules: tourism/marble/BPO)
- Total: ₱18M over 2 years

**LGU Co-Funding:** 20% of operating costs (Years 1-2)
- Provincial: ₱1.5M/year (teacher training, device procurement)
- Municipalities: ₱100K/year each (internet connectivity, venue costs)

**CSV Role:** Technical implementation partner + platform operator
- Deploy learning platform to 85 public schools + RSU
- Train 450 teachers on digital pedagogy + AI tools
- Deliver 5,000 student enrollments in skills training modules
- Provide 24/7 technical support + platform updates

**Sustainability (Post-Pilot):**
- DepEd absorbs platform as part of national LMS (scales to other regions)
- LGU co-funding increases to 50% (provincial + municipal budgets)
- National subsidy covers 50% (DepEd allocation for digital learning)
- Skills training revenue: Employers pay ₱5K per trainee for custom programs

---

## 5. Implementation Roadmap

### Month 1: Partnership & Site Assessment
- **Week 1:** Stakeholder briefing (Provincial Governor, 17 Municipal Mayors, SP members)
- **Week 2:** Community consultation (barangay captains, teachers, business owners)
- **Week 3:** Site assessment (internet connectivity, LGU IT capacity, school infrastructure)
- **Week 4:** MOU signing + pilot municipality selection (Romblon town + 2 others)

### Months 2-3: Deployment & Training
- **Platform Setup:** Cloud infrastructure (AWS Manila region), database migration, AI training
- **Pilot Rollout:** 3 municipalities go live (Romblon, Odiongan, San Agustin)
- **Training:** 150 LGU staff, 50 teachers, 100 barangay officials (3-day workshops)
- **Content Creation:** Romblomanon/Onhan/Asi language packs, local tourism modules

### Months 4-6: Pilot Operations & Iteration
- **Live Operations:** 10,000+ citizens using AI helpdesk, 500+ permits processed
- **Data Collection:** User feedback surveys (NPS), system performance (uptime, response times)
- **Iteration:** Bug fixes, UI improvements, additional features based on feedback
- **Mid-Pilot Review:** CSV + LGU + DICT/DepEd stakeholders assess progress

### Months 7-12: Province-Wide Rollout
- **17-Municipality Expansion:** Remaining 14 municipalities onboarded (phased rollout)
- **EdTech Integration:** 85 public schools + RSU go live with learning platform
- **National Showcase:** DICT/DepEd invite other provinces to study Romblon model
- **Sustainability Planning:** LGU budget allocation for Years 2-3, BOT transfer preparations

---

## 6. Success Metrics (6-Month Pilot)

### Governance (LGU AI Platform)
- **10,000+ citizens** using AI helpdesk (calls to municipal offices drop 60%)
- **500+ business permits** processed digitally (EODB compliance: 3-day average)
- **Zero data breaches** (DPIA-compliant, ISO 27001 aligned)
- **99.5% uptime** (24/7 availability SLA met)
- **80% citizen satisfaction** (NPS >60)

### Education (EdTech Ecosystem)
- **5,000+ students** enrolled on learning platform (58% of target schools)
- **450 teachers** trained on digital pedagogy (100% of pilot schools)
- **1,000+ skills training completions** (tourism/marble/BPO micro-credentials)
- **40% improvement** in student engagement (teacher-reported, pre/post surveys)
- **25% reduction** in dropout rates (pilot schools vs provincial baseline)

### Economic Impact
- **3x increase** in business registrations (EODB removes friction)
- **₱8M/year savings** for LGUs (staff overtime, paper costs, faster procurement)
- **200 new jobs** created (skilled workforce via EdTech → hired by tourism/marble employers)
- **25% reduction** in youth out-migration (local opportunities via skills training)

---

## 7. Risk Mitigation

### Technical Risks
- **Low internet connectivity:** Offline-capable mobile apps, SMS fallback for AI helpdesk
- **Staff resistance:** Change management workshops, "AI as assistant not replacement" messaging
- **Data privacy concerns:** DPIA from Day 1, citizen consent mechanisms, Data Privacy Officer hired

### Financial Risks
- **LGU budget constraints:** Phased payment plan, national agency grants (DICT/DepEd) cover 60% of costs
- **Revenue shortfall:** CSV maintains operations even if LGU payments delayed (contractual commitment)

### Political Risks
- **Election cycle disruption (2025):** MOU signed pre-election, endorsed by all mayoralty candidates
- **Inter-LGU coordination challenges:** Provincial government as central coordinator, not individual municipalities

### Operational Risks
- **Vendor lock-in:** Open-source core (Moodle, PostgreSQL), CSV transfers all IP at Year 3
- **Talent shortage:** Remote operations center in Manila (CSV staff), gradual knowledge transfer to Romblon IT team

---

## 8. National Scalability Thesis

### Why Romblon Proves the Model

**Replicable Geography:**
- 463 island municipalities in PH mirror Romblon's constraints (limited connectivity, small budgets)
- Success here = template for Palawan, Sulu, Catanduanes, Guimarás, Dinagat Islands

**Cost Efficiency:**
- Per-capita deployment cost: ₱100/citizen (vs ₱250 in Metro Manila pilots)
- Island provinces can afford Romblon's pricing model (₱150K/municipality/month)

**Partnership Template:**
- Provincial + 17 municipal LGUs = multi-tier governance reference
- DICT + DepEd + DOST + LGU co-funding = sustainable financing blueprint

**Validation for National Programs:**
- **DICT eGov PH System:** Romblon validates cloud-based LGU services at scale
- **DepEd Digital Transformation Roadmap:** Proves AI learning works in under-resourced schools
- **NEDA Philippine Development Plan 2023-2028:** Demonstrates inclusive digital transformation

### Target: 50 Island Provinces by 2028

**Phase 1 (2026):** Romblon pilot (302K citizens)  
**Phase 2 (2027):** 5 island provinces (1.2M citizens) — Palawan, Guimarás, Catanduanes, Dinagat, Camiguin  
**Phase 3 (2028):** 44 additional provinces (3.8M citizens) — full island province coverage

**Revenue Projection (2028):**
- 50 provinces × ₱30M/year (avg) = ₱1.5B annual recurring revenue
- CSV retains 40% post-scale (₱600M/year), provinces retain 60% (reinvested in digital infra)

---

## 9. Why CSV × Likha Labs

### CSV (Climate Smart Ventures) — Lead Proponent
- **Track Record:** Advisory to DOE, DOF, PPP Center, LGUs on climate projects
- **Policy Expertise:** Deep relationships with DICT, DepEd, DOST, NEDA
- **Business Development:** Pipeline of 50+ LGU relationships (mayors, governors, SP members)
- **Grant Access:** Proven ability to secure DICT/DepEd/DOST funding (₱60M+ mobilized to date)

### Likha Labs — Technology Partner
- **Proven Platforms:** CSV Radar (live), CSV Orbit (production), Accord (70% complete)
- **Fusion Engineering Methodology:** Structured transformation framework (Confuse → Infuse → Diffuse → Refuse)
- **Governance-by-Design:** DPIA-compliant, Cloud First aligned, audit trails, RBAC/SSO, ISO 27001 mapping
- **Deployment Speed:** 4-6 weeks from MOU to pilot launch (vs 6-12 months industry standard)

### Partnership Strengths
- **Complementary Skills:** CSV = policy/BD, Likha Labs = product/engineering
- **Shared Values:** Humanized progress, inclusive growth, transferable capabilities (not vendor lock-in)
- **Regional Focus:** Philippine-first, SEA expansion (not foreign tech parachuting in)
- **Sustainability Commitment:** Full IP transfer at Year 3 (provinces own their digital infrastructure)

---

## 10. Next Steps

### Immediate Actions (Next 30 Days)

**Week 1:**
- Finalize pitch deck (this document + HTML presentation)
- Secure meeting with Romblon Provincial Governor (Hon. Trina Alejandra Q. Firmalo-Fabic)
- Engage DILG Region 4B for endorsement

**Week 2:**
- Stakeholder briefing in Romblon (Governor, mayors, SP, business sector, teachers)
- Site visit: 3 municipalities (Romblon, Odiongan, San Agustin) + 5 schools + RSU
- Community consultation: 10 barangays (citizens, captains, SK officials)

**Week 3:**
- MOU drafting (legal review by PPP Center, Provincial Legal Office)
- Pilot municipality selection (based on digital readiness, mayor buy-in, barangay coverage)
- Budget allocation coordination (Provincial, Municipal, DICT, DepEd)

**Week 4:**
- MOU signing ceremony (Provincial Capitol, media coverage)
- Kickoff meeting with DICT Region 4B, DepEd Romblon Division Office
- Deployment planning workshop (CSV + Likha Labs + LGU IT teams)

### Key Contacts for Outreach

**Romblon Provincial Government:**
- Governor: Hon. Trina Alejandra Q. Firmalo-Fabic (Liberal Party)
- Vice Governor: Hon. Armando Gutierrez (Partido Federal ng Pilipinas)
- Provincial Planning & Development Officer (PPDO)

**DICT Region 4B:**
- Regional Director: Dir. Marianito E. Borja
- IT Officers for Romblon province

**DepEd Romblon Division:**
- Schools Division Superintendent (SDS)
- Education Program Supervisors (EPS) for ICT, Curriculum

**DILG Region 4B:**
- Regional Director (for LGU endorsement)
- Provincial Director for Romblon

---

## Appendix: Legal & Regulatory Compliance

### Applicable Laws & Policies

**Governance & Procurement:**
- RA 11966 (PPP Code, 2023) — Sec 10: Unsolicited proposal procedures, timelines, approving body
- RA 12009 (Procurement Act, 2024) — Sec 22: E-procurement, audit trails, PhilGEPS interconnectivity
- RA 11032 (EODB, 2018) — 3-day simple permits, 20-day complex permits, digital processing
- DICT Cloud First Policy (2020) — Cloud adoption, data classification, residency requirements

**Data Privacy & Security:**
- RA 10173 (Data Privacy Act, 2012) — Sec 11(d): Legitimate processing, Sec 20: Security measures
- NPC Circular 16-01: DPIA guidelines for government systems
- NPC Advisory Opinion 2018-024: Cloud computing and cross-border data transfer

**Education:**
- RA 11055 (PSED, 2018) — Free tertiary education, quality assurance
- RA 10929 (Free Internet, 2017) — Public WiFi in schools, government offices, public spaces
- DepEd Order No. 42, s. 2020 — Digital Transformation Roadmap 2023-2028

### Compliance Measures Embedded in Platform

**DPIA-by-Default:**
- Citizen consent mechanisms (opt-in for AI helpdesk, explicit consent for data sharing)
- Data minimization (only collect necessary fields for each service)
- Retention policies (auto-delete after legal requirements met: 5 years for permits, 3 years for inquiries)

**Cloud First Alignment:**
- AWS Manila region (data residency within PH)
- Government Cloud certification (DICT-approved infrastructure)
- Backup and disaster recovery (RTO <4 hours, RPO <1 hour)

**Audit Trails:**
- Immutable logs for all transactions (permit approvals, budget changes, citizen inquiries)
- Cryptographic checksums (SHA-256) for document integrity
- Real-time audit dashboards for COA, DILG, provincial auditors

**RBAC & SSO:**
- Role-based access control (Mayor, Department Heads, Staff, Citizens have different permissions)
- Single Sign-On via PhilSys/eGov PH credentials (future integration)
- Multi-factor authentication for admin accounts

---

**END OF BRIEF**

---

**Contact:**

**Climate Smart Ventures (CSV)**  
Lead Proponent  
Email: [contact information]  
Mobile: [contact information]

**Likha Labs**  
Technology Partner  
Email: [contact information]  
Mobile: [contact information]

**Prepared by:** Martin Banaria (CSV BD Lead / Likha Labs Founder)  
**Version:** 1.0  
**Date:** January 14, 2026
