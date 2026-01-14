# Romblon Pitch Presentation — Improvement Plan v1.2

**Created:** January 15, 2026  
**Target Version:** v1.2  
**Current Version:** v1.1  
**Status:** In Progress

---

## Executive Summary

This improvement plan consolidates findings from:
1. **QA Content Review** — Data accuracy, claim verification, naming consistency
2. **UI/UX Audit (Agent Architect)** — Comprehensive accessibility, visual design, interaction review
3. **Scope Expansion** — Enhanced EdTech with Career Pathways + Tech/AI courses

**Overall Assessment:** Current presentation scores **78/100** (Good). Target score: **90+/100** after improvements.

---

## Improvement Categories

### Phase 1: Critical Fixes (Before Next Presentation)
| ID | Issue | Priority | Effort | Status |
|----|-------|----------|--------|--------|
| C-1 | Focus states missing on navigation buttons | Critical | 5 min | Pending |
| C-2 | Aria-labels missing on navigation buttons | Critical | 2 min | Pending |
| C-3 | Low contrast muted text (#888 → #9a9a9a) | High | 1 min | Pending |
| C-4 | External Unsplash images (offline failure risk) | High | 15 min | Pending |
| C-5 | Pasig City claims need softer language | High | 5 min | Pending |

### Phase 2: Content Expansion (EdTech Scope)
| ID | Issue | Priority | Effort | Status |
|----|-------|----------|--------|--------|
| E-1 | Add Career Pathways section to EdTech | High | 30 min | Pending |
| E-2 | Add Tech/AI Courses module | High | 30 min | Pending |
| E-3 | Update Slide 6 with expanded scope | High | 20 min | Pending |
| E-4 | Update persona (Entrepreneur Carlo) with tech hiring | Medium | 10 min | Pending |

### Phase 3: Accessibility & UX Polish
| ID | Issue | Priority | Effort | Status |
|----|-------|----------|--------|--------|
| A-1 | Add Space bar navigation | Medium | 2 min | Pending |
| A-2 | Increase mobile touch targets to 44×44px | Medium | 2 min | Pending |
| A-3 | Add aria-live to slide counter | Medium | 3 min | Pending |
| A-4 | Improve alt text on 3 images | Medium | 5 min | Pending |
| A-5 | Increase .mono font size to 0.9rem | Medium | 1 min | Pending |
| A-6 | Increase footnote contrast (#555 → #888) | Medium | 1 min | Pending |

### Phase 4: Nice-to-Have Enhancements
| ID | Issue | Priority | Effort | Status |
|----|-------|----------|--------|--------|
| N-1 | Add number key slide navigation (1-0) | Low | 10 min | Pending |
| N-2 | Add tablet breakpoint (992px) | Low | 15 min | Pending |
| N-3 | Split dense slides (5, 9) | Low | 45 min | Pending |
| N-4 | Update README with v1.2 changes | Low | 10 min | Pending |

---

## Detailed Implementation Guide

### C-1: Focus States for Navigation Buttons

**Location:** Line 33-34 (CSS)

**Current:**
```css
.btn-nav:hover{background:rgba(255,255,255,0.1);border-color:var(--accent-color);color:var(--accent-color)}
```

**Add:**
```css
.btn-nav:focus-visible{outline:2px solid var(--accent-color);outline-offset:3px;background:rgba(255,255,255,0.15)}
```

---

### C-2: Aria-Labels for Navigation Buttons

**Location:** Lines 427, 429 (HTML)

**Current:**
```html
<button class="btn-nav" onclick="prevSlide()">←</button>
<button class="btn-nav" onclick="nextSlide()">→</button>
```

**Replace with:**
```html
<button class="btn-nav" onclick="prevSlide()" aria-label="Previous slide">←</button>
<button class="btn-nav" onclick="nextSlide()" aria-label="Next slide">→</button>
```

---

### C-3: Muted Text Contrast Fix

**Location:** Line 8 (CSS :root)

**Current:**
```css
--muted-text:#888;
```

**Replace with:**
```css
--muted-text:#9a9a9a;
```

**Also update footnote (Line 18):**
```css
.footnote{font-size:0.7rem;color:#888;...} /* Was #555 */
```

---

### C-4: Replace External Images

**Location:** Lines 52, 130, 228

**Option A (Recommended): Use placeholder SVG patterns**
Replace Unsplash URLs with inline SVG data URIs that match the Operational Noir theme.

**Option B: Download and embed as base64**
Convert images to base64 and embed directly in the HTML.

**Option C: Use local files**
Download images to `/images/` folder and reference locally.

**Recommended Images to Replace:**
| Line | Current URL | Suggested Replacement |
|------|-------------|----------------------|
| 52 | unsplash office photo | Abstract grid pattern (SVG) or Romblon aerial photo |
| 130 | unsplash island photo | Romblon coastline photo (if available) |
| 228 | unsplash students photo | Filipino classroom photo (if available) |

---

### C-5: Soften Pasig City Claims

**Location:** Lines 205-209 (Slide 5)

**Current:**
```html
<li>✓ 50-70% reduction in staff document retrieval time</li>
<li>✓ 30-40% reduction in walk-in clarification requests</li>
```

**Replace with:**
```html
<li>✓ Significant reduction in staff document retrieval time</li>
<li>✓ Fewer walk-in clarification requests reported</li>
```

**Or add qualifier:**
```html
<li>✓ Up to 50-70% reduction in document retrieval time (pilot data)</li>
<li>✓ Up to 30-40% reduction in walk-in requests (early results)</li>
```

---

## EdTech Scope Expansion (E-1 to E-4)

### New EdTech Vision: Career-First, Tech-Focused

**Current Scope (v1.1):**
- AI-adaptive learning (K-12, tertiary)
- Skills training (tourism, marble, BPO-ready)
- Review & certification platform (TESDA-aligned)
- Teacher professional development

**Expanded Scope (v1.2):**

#### Career Pathways Platform
A structured journey from learning to employment:

1. **Skills Assessment** — AI-powered aptitude and interest mapping
2. **Learning Paths** — Curated courses based on career goals
3. **Certification** — Industry-recognized credentials
4. **Job Matching** — Direct connections to local and remote employers
5. **Career Tracking** — Post-placement success monitoring

#### Tech & AI Courses Module
Focus on high-demand, industry-agnostic skills:

| Category | Courses | Target Jobs |
|----------|---------|-------------|
| **AI Fundamentals** | Prompt Engineering, AI Tools for Work, Data Literacy | Any industry (AI-augmented roles) |
| **Digital Skills** | Google Workspace, Microsoft 365, Canva, Basic Coding | Admin, Marketing, Operations |
| **Tech Operations** | Help Desk, IT Support, Cloud Basics | IT Support, Tech Operations |
| **Data & Analytics** | Excel Advanced, Google Sheets, Basic SQL, Dashboarding | Analyst roles across industries |
| **Remote Work Ready** | Virtual Collaboration, Time Management, Freelancing 101 | BPO, Freelance, Remote roles |
| **Industry-Specific Tech** | Tourism Tech (booking systems), Marble CAD/CAM basics | Local industry advancement |

#### Industry Landing Zones
Skills that land jobs across multiple sectors:

| Skill | Tourism | Marble | BPO | Government | Healthcare |
|-------|---------|--------|-----|------------|------------|
| AI Tools | ✓ | ✓ | ✓ | ✓ | ✓ |
| Data Entry | ✓ | ✓ | ✓ | ✓ | ✓ |
| Customer Service | ✓ | | ✓ | ✓ | ✓ |
| Digital Marketing | ✓ | ✓ | ✓ | | |
| Basic Coding | | ✓ | ✓ | ✓ | |

---

### Slide 6 Rewrite (EdTech Deep Dive)

**Replace current Slide 6 content with:**

```html
<!-- SLIDE 6: EdTech LMS Deep Dive — UPDATED -->
<div class="slide" id="slide-6">
  <div class="split-layout">
    <div class="mockup-container">
      <img src="[LOCAL_IMAGE]" alt="Filipino students engaged with laptops in a classroom setting" class="mockup-img" style="opacity:.8">
    </div>
    <div>
      <span class="blur-pill">EDTECH LMS PLATFORM</span>
      <h2>From Learning to Earning</h2>
      <p style="margin-top:1.5rem">Career-first learning platform with AI-powered pathways to employment.</p>
      
      <h3 style="color:#fff;font-size:1.3rem;margin:2rem 0 1rem">Career Pathways</h3>
      <ul style="list-style:none;color:#ccc;font-size:.95rem;line-height:1.8">
        <li>• AI-powered skills assessment & career mapping</li>
        <li>• Personalized learning paths based on job goals</li>
        <li>• Direct job matching with local & remote employers</li>
        <li>• Post-placement success tracking</li>
      </ul>

      <h3 style="color:#fff;font-size:1.3rem;margin:2rem 0 1rem">Tech & AI Skills (Industry-Agnostic)</h3>
      <ul style="list-style:none;color:#ccc;font-size:.95rem;line-height:1.8">
        <li>• AI Fundamentals: Prompt engineering, AI tools for work</li>
        <li>• Digital Skills: Google Workspace, Canva, basic coding</li>
        <li>• Data & Analytics: Excel, SQL basics, dashboarding</li>
        <li>• Remote Work Ready: Virtual collaboration, freelancing</li>
      </ul>

      <h3 style="color:#fff;font-size:1.3rem;margin:2rem 0 1rem">Industry-Specific Tracks</h3>
      <ul style="list-style:none;color:#ccc;font-size:.95rem;line-height:1.8">
        <li>• Tourism: Hospitality tech, booking systems, guest experience</li>
        <li>• Marble: CAD/CAM basics, quality control, export standards</li>
        <li>• BPO: English proficiency, typing, customer service</li>
        <li>• Government: eGov systems, citizen service, data privacy</li>
      </ul>
    </div>
  </div>
</div>
```

---

### Slide 4 Update (Two Platforms Overview)

**Update EdTech card (lines 154-165) to reflect new scope:**

```html
<div class="stat-card" style="border-left:4px solid var(--secondary-accent)">
  <span class="mono" style="color:var(--secondary-accent)">PLATFORM 2: EDUCATION</span>
  <h3 style="color:#fff;font-size:1.8rem;margin:1rem 0">EdTech LMS</h3>
  <p style="font-size:1rem;margin-bottom:1.5rem;color:#aaa">Career Pathways, Tech Skills & Industry Certification</p>
  <ul style="list-style:none;padding:0;text-align:left;font-size:.95rem;line-height:1.8">
    <li>✓ AI-powered career pathway mapping</li>
    <li>✓ Tech & AI skills (industry-agnostic)</li>
    <li>✓ Industry tracks: Tourism, Marble, BPO, Gov</li>
    <li>✓ Direct job matching with employers</li>
    <li>✓ TESDA-aligned certification</li>
  </ul>
</div>
```

---

### Persona Update (Entrepreneur Carlo)

**Location:** Lines 283-289 (Slide 7)

**Update to reflect tech hiring:**

```html
<div class="stat-card">
  <div style="width:60px;height:60px;background:rgba(255,77,77,0.1);border-radius:50%;display:flex;align-items:center;justify-content:center;margin-bottom:1rem;font-size:1.8rem">🧑‍💼</div>
  <p class="mono">ENTREPRENEUR CARLO</p>
  <h4 style="color:#fff;margin:.5rem 0">Marble Workshop Owner</h4>
  <p style="font-size:.9rem;margin-top:1rem"><strong>Needs:</strong> Fast permits, tech-savvy workforce, AI tools for business.</p>
  <p style="font-size:.85rem;color:#fff;margin-top:1rem"><strong>Both platforms:</strong> Digital permits + hire platform-trained workers with CAD, data, and AI skills.</p>
</div>
```

---

## Accessibility & UX Polish (A-1 to A-6)

### A-1: Space Bar Navigation

**Location:** Line 440 (JavaScript)

**Current:**
```javascript
document.addEventListener('keydown',e=>{if(e.key==='ArrowRight')nextSlide();if(e.key==='ArrowLeft')prevSlide()});
```

**Replace with:**
```javascript
document.addEventListener('keydown',e=>{if(e.key==='ArrowRight'||e.key===' ')nextSlide();if(e.key==='ArrowLeft')prevSlide();if(e.key===' ')e.preventDefault()});
```

---

### A-2: Mobile Touch Targets

**Location:** Line 40 (CSS @media)

**Current:**
```css
.btn-nav{width:40px;height:40px;font-size:1rem}
```

**Replace with:**
```css
.btn-nav{width:44px;height:44px;font-size:1rem}
```

---

### A-3: Aria-Live for Slide Counter

**Location:** Line 428 (HTML)

**Current:**
```html
<span class="mono" id="slide-counter" style="display:flex;align-items:center;color:var(--muted-text)">1 / 10</span>
```

**Replace with:**
```html
<span class="mono" id="slide-counter" aria-live="polite" style="display:flex;align-items:center;color:var(--muted-text)">1 / 10</span>
```

---

### A-4: Improved Alt Text

**Location:** Lines 52, 130, 228

| Line | Current | Improved |
|------|---------|----------|
| 52 | "Legacy LGU Operations" | "Modern office workspace symbolizing digital transformation potential for local government" |
| 130 | "Island Community" | "Aerial view of Philippine island coastline representing Romblon's geographic context" |
| 228 | "Students Learning" | "Filipino students collaborating with laptops in a classroom, representing EdTech adoption" |

---

### A-5: Mono Font Size Increase

**Location:** Line 15 (CSS)

**Current:**
```css
.mono{font-family:var(--font-mono);color:var(--secondary-accent);font-size:0.8rem;...}
```

**Replace with:**
```css
.mono{font-family:var(--font-mono);color:var(--secondary-accent);font-size:0.9rem;...}
```

---

### A-6: Footnote Contrast Fix

**Location:** Line 18 (CSS)

**Current:**
```css
.footnote{font-size:0.7rem;color:#555;...}
```

**Replace with:**
```css
.footnote{font-size:0.8rem;color:#888;...}
```

---

## Validation Checklist

### Before Marking Complete

- [ ] All Critical (C-1 to C-5) items resolved
- [ ] EdTech content (E-1 to E-4) updated in Slides 4, 6, 7
- [ ] Accessibility fixes (A-1 to A-6) applied
- [ ] Test keyboard navigation (Tab, Arrow keys, Space)
- [ ] Test on mobile device (iOS Safari, Android Chrome)
- [ ] View in offline mode (disconnect WiFi, reload)
- [ ] Run through WAVE or axe DevTools for A11Y audit
- [ ] Proofread all new content for typos
- [ ] Update version number to v1.2 in `<title>` tag
- [ ] Update README.md with v1.2 changelog

---

## Version History

| Version | Date | Changes |
|---------|------|---------|
| v1.0 | Jan 14, 2026 | Initial proposal version |
| v1.1 | Jan 14, 2026 | Removed pricing, added Gyud.AI, intro tone |
| v1.2 | Jan 15, 2026 | (Planned) A11Y fixes, EdTech expansion, UI polish |

---

**Plan Author:** Claude (AI Assistant)  
**Reviewed By:** Martin Banaria  
**Target Completion:** Before next presentation
