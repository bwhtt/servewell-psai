# Methodology

## How We Turn Data Into Scores

The Public Servant Appreciation Index transforms publicly available data—salaries, vacancy rates, recognition events, budget documents—into comparable scores that reveal how well states support their public workforce.

This page explains how we collect data, ensure accuracy, and calculate scores. Everything described here is transparent, replicable, and open for review.

---

## The Assessment Process: Step by Step

### Step 1: Data Collection

We gather data from authoritative sources for each state:

**Government databases**:
- Bureau of Labor Statistics (salary data)
- State budget documents (appropriations, IT spending)
- HR department reports (turnover, tenure, benefits)
- Legislative fiscal analyses (vacancy rates, program details)

**Public records**:
- Salary transparency portals
- Pension system documentation
- Employee handbook and policy documents

**Polling organizations**:
- University-sponsored public opinion polls
- Reputable polling firms with transparent methodology

**Recognition infrastructure**:
- Governor's office press releases and proclamations
- State HR department award programs
- Agency websites and news coverage
- Humans of Public Service (HOPS) platform

**Search requirements**: Minimum time thresholds ensure thorough data collection (e.g., 2.5 hours searching for recognition events, 2 hours for training budgets). This prevents incomplete assessments.

---

### Step 2: Data Validation

Before any data becomes part of a state's score, it undergoes multiple validation checks:

**Reality checks**: Does this number make sense for this type of state?  
*Example*: If Massachusetts shows a median salary of $49,000, we investigate—that's too low for a high cost-of-living state with strong unions.

**Source verification**: Can we confirm this data is accurate and current?  
*Example*: Document exact URL, date accessed, filters applied, sample size.

**Cross-state comparison**: Does this state's performance fit expected patterns?  
*Example*: Right-to-work states typically show 85-110% salary ratios. A 130% ratio triggers investigation.

**Approval checkpoint**: After collecting salary data, analysts must submit for reviewer approval before proceeding. This catches errors in 30 minutes instead of after 5 hours of work.

---

### Step 3: Component Scoring

Each dimension contains multiple components that are scored individually:

**Example: Dimension 1 (Competitive Compensation) has three components:**

1. **Salary Competitiveness (0-70 points)**
   - Calculate median salary ratio: (state employee median) ÷ (private sector median)
   - Adjust for cost of living using Regional Price Parity indices
   - Convert ratio to points using standardized scale

2. **Cost of Living Adjustment (0-15 points)**
   - Compare state cost of living to national average
   - Higher scores for states where salaries go further

3. **Benefits Quality (0-15 points)**
   - Evaluate pension (defined-benefit vs. hybrid vs. defined-contribution)
   - Health insurance employer contribution percentage
   - Paid leave policies
   - Additional perks (tuition, loan forgiveness, transit)

Components are scored using rubrics and formulas detailed in the complete framework documentation.

---

### Step 4: Dimension Calculation

Component scores combine using fixed, weighted formulas:

**Dimension 1 (Compensation)** = (0.40 × Salary) + (0.35 × COL) + (0.25 × Benefits)  
**Dimension 2 (Workforce Health)** = (0.40 × Retention) + (0.35 × Vacancy) + (0.25 × Tenure)  
**Dimension 3 (Public Perception)** = (0.70 × Trust) + (0.30 × Events)  
**Dimension 4 (Investment)** = (0.50 × Training) + (0.30 × Prof Dev) + (0.20 × Tech)  
**Dimension 5 (Recognition)** = (0.40 × HOPS) + (0.35 × Programs) + (0.25 × Observances)

**Critical rule**: These formulas are **fixed across all states**. We cannot modify weights even if it would improve a state's score. Consistency enables comparison.

---

### Step 5: Composite Score

Dimension scores combine into a final 0-100 composite score:

**Final Score** = (0.30 × D1) + (0.28 × D2) + (0.22 × D3) + (0.15 × D4) + (0.05 × D5)

This weighted average reflects the relative importance of each dimension for making public service sustainable.

---

### Step 6: Tier Assignment

Final scores fall into three fixed tiers:

- **Leading**: 75-100 points
- **Developing**: 50-74 points  
- **Emerging**: 0-49 points

These thresholds don't shift as more states are added. A "Developing" score means the same thing whether we've assessed 5 states or 50.

---

## Data Quality Standards

### The Three Quality Flags

Every data point in every state report carries one of three flags:

**✅ Verified** – Direct from authoritative government source, confirmed accurate  
*Example*: Virginia salary data from Virginia DataPoint database

**⚠️ Estimated** – Calculated from partial data using documented methodology  
*Example*: Maryland's employer health premium contribution (75%) estimated from contract documents

**❌ Data Not Published** – Could not be found despite extensive searching  
*Example*: Most states don't publish consolidated training budgets → scored as 0

**Why this matters**: You deserve to know our confidence level in every finding. When data is missing, we say so rather than guessing.

---

### When Data Is Missing

**Our policy**: If data genuinely cannot be found after thorough searching, we:

1. Document all search attempts (URLs, time spent, locations checked)
2. Score the component as **zero**
3. Flag it as **"DATA NOT PUBLISHED"** in the report
4. Recommend transparency improvements in the "Next Steps" section

**We do not estimate or extrapolate missing data.** This creates incentive for states to publish information rather than rewarding opacity with estimated scores.

---

## Methodological Consistency

### Why Fixed Formulas Matter

Every state uses **identical formulas**. We cannot:
- ❌ Adjust weights because a component scored zero
- ❌ Modify formulas to make results "fairer"
- ❌ Use different calculation methods for different states
- ❌ Cherry-pick data sources that favor certain states

**Why**: Maryland (67.9), Massachusetts (67.1), Virginia (64.4), Washington (65.5), and North Carolina (61.7) are comparable **only because** they were assessed identically. Changing methodology breaks comparability.

---

### Formula Verification Checklist

Before finalizing any state assessment, analysts verify:

✅ All six formulas match framework exactly  
✅ No unauthorized weight modifications  
✅ All calculations verified manually  
✅ Excel formulas contain no errors  
✅ Dimension scores sum correctly to composite

One state (Virginia, initially) modified formulas. We caught and corrected this, reducing their score by 1.3 points but maintaining methodological integrity.

---

## AI Collaboration in Methodology

We use AI tools transparently:

**ChatGPT handles data collection**:
- Searches government databases and documents
- Extracts quantitative data (salaries, rates, budgets)
- Documents sources with URLs and dates
- Follows minimum search time protocols

**Claude assists with analysis**:
- Reviews collected data for consistency
- Flags implausible results for verification
- Helps structure findings into narratives
- Identifies patterns across states

**Human oversight maintains control**:
- Designs framework and formulas
- Approves all data before finalization
- Makes interpretation and recommendation decisions
- Verifies sources and catches AI errors
- Ensures methodological consistency

**All prompts, quality controls, and AI collaboration methods are documented on GitHub.**

---

## Quality Assurance: How We Prevent Errors

Rigorous quality control evolved from real mistakes we caught and fixed. Key safeguards include:

**5 Reality Checks on Salary Data** – Catches errors like Massachusetts's initial $49,000 median (actual: $73,645)

**Approval Checkpoints** – Reviewer must approve salary data before analysis proceeds

**Minimum Search Times** – Prevents incomplete data collection (2.5 hours for recognition, 2 hours for training)

**Formula Lock Requirements** – Prevents unauthorized methodology changes

**Cross-State Comparison** – Flags outliers that don't fit expected patterns

**[See complete quality control procedures →](link-to-quality-summary)**

---

## Our Track Record

Across five states assessed with framework v2.2:

**Formula Compliance**: 100% ✅  
**Data Accuracy**: Zero major errors after checkpoints implemented ✅  
**Methodology Consistency**: 100% identical formulas ✅  
**Source Documentation**: Every data point traceable ✅

---

## Methodology Transparency

Every element of our methodology is documented and available for review:

**[Complete Framework v2.2](link-to-full-framework)** – All formulas, weights, scoring rubrics  
**[Quality Control Procedures](link-to-full-qc)** – Every checkpoint and verification step  
**[Framework Change History](link-to-change-history)** – How methodology evolved  
**[GitHub Repository](link-to-github)** – View prompts, data, and calculations  
**[State Reports](link-to-reports)** – See methodology in action with source citations

---

## Limitations & What We Don't Measure

**This methodology measures what's quantifiable and comparable:**
- Salaries, benefits, leave policies
- Vacancy rates, retention, tenure
- Public trust polling data
- Budget appropriations for training and technology
- Documented recognition events and programs

**This methodology doesn't measure:**
- Workplace culture or leadership quality
- Whether work feels meaningful
- Geographic variations within states
- Political interference or job security
- Actual workload or understaffing severity

These factors matter but are harder to measure consistently across states. We welcome suggestions for expanding methodology while maintaining rigor.

---

## Continuous Improvement

Methodology evolves based on lessons learned:

- **v2.0**: Added data quality standards and transparency requirements
- **v2.1**: Added formula protection and minimum search times  
- **v2.2**: Added reality checks and approval checkpoints (current)

Future versions will address new challenges as they emerge. All changes are documented in the Framework Change History.

---

## Questions or Concerns?

If you believe our methodology should be improved, **[we want to hear from you](link-to-feedback)**:

- **[Contact Form](link)** – General methodology questions
- **[GitHub Issues](link)** – Specific technical suggestions with evidence
- **[Collaboration](link)** – Join as a methodology reviewer or validator

This work is stronger when informed by diverse expertise—researchers, public servants, statisticians, policy experts, and citizens.

---

**[Explore the Framework →](#) | [View State Reports →](#) | [See Quality Controls →](#)**
-e 
---

# How We Ensure Data Quality

Every state assessment undergoes rigorous quality control to ensure accuracy, consistency, and comparability. These safeguards evolved from real mistakes we caught and fixed—making the methodology stronger with each state analyzed.

---

## Our Quality Philosophy

**Catch errors early** – Better to spend 10 minutes verifying data than 5 hours redoing analysis.

**Trust but verify** – Even authoritative sources can have errors. Every data point gets validated.

**Consistency over optimization** – Identical methodology across all states matters more than making any single state's score look better.

**Transparency over perfection** – We openly acknowledge data limitations rather than hiding them.

---

## 5 Reality Checks on Every State

### 1. Salary Range Check
**What we test**: Does the median salary fall within expected ranges for this type of state?

**Example ranges**:
- High cost-of-living + strong unions (MA, WA): $60,000-$85,000 expected
- Moderate cost-of-living + right-to-work (VA, NC): $50,000-$70,000 expected

**Red flags**:
- ❌ Median under $45,000 (too low for any state)
- ❌ Median over $95,000 (likely filtering error—may have captured only executives)

**Why it matters**: Massachusetts initially showed $49,598 median salary. Reality check caught the error—actual median was $73,645. This prevented a 5-point scoring mistake.

---

### 2. Salary Ratio Check
**What we test**: Does the public-to-private wage ratio make sense for this state's labor market?

**Expected ratios**:
- Strong union states: 95%-125% of private sector
- Right-to-work states: 85%-110% of private sector
- Tech-heavy private sectors (WA, MA): May suppress ratio despite high absolute pay

**Red flags**:
- ❌ Ratio below 70% (likely wrong comparison group)
- ❌ Ratio above 130% (likely data error)

**Why it matters**: Ensures apples-to-apples comparisons across different state economies.

---

### 3. Data Source Verification
**What we document for every data point**:
- ✅ Exact URL of source
- ✅ Date accessed
- ✅ Filters applied (full-time only, state employees only, fiscal year)
- ✅ Number of employees in dataset
- ✅ Which employee categories were excluded (local government, K-12, higher education)

**Why it matters**: Prevents common errors like accidentally including local government employees or school districts, which skew results unpredictably.

---

### 4. Cross-State Comparison
**What we test**: Does this state's performance fit expected patterns given its characteristics?

**Example**: Right-to-work states typically show 85-110% salary ratios. If North Carolina suddenly showed 130%, we'd investigate why they're an outlier.

**Why it matters**: Catches data anomalies by comparing similar states to each other.

---

### 5. Formula Compliance Check
**What we verify**: All six formulas (five dimensions + composite score) match the framework exactly.

**Non-negotiable formulas**:
- Dimension 1: (0.40 × Salary) + (0.35 × COL) + (0.25 × Benefits)
- Dimension 2: (0.40 × Retention) + (0.35 × Vacancy) + (0.25 × Tenure)
- Dimension 3: (0.70 × Trust) + (0.30 × Events)
- Dimension 4: (0.50 × Training) + (0.30 × Prof Dev) + (0.20 × Tech)
- Dimension 5: (0.40 × HOPS) + (0.35 × Programs) + (0.25 × Observances)
- Composite: (0.30 × D1) + (0.28 × D2) + (0.22 × D3) + (0.15 × D4) + (0.05 × D5)

**Why it matters**: Virginia's initial analysis modified formulas, making their score incomparable to Maryland. We caught and corrected this, losing 1.3 points but gaining methodological integrity.

---

## Mandatory Approval Checkpoint

**After collecting salary data, analysis STOPS.**

The analyst must submit salary data for reviewer approval before continuing. This checkpoint includes:
- Median salary figure
- Public-to-private ratio
- Results of all five reality checks
- Any concerns or anomalies

**Why it matters**: Prevents building a 5-hour analysis on a flawed 30-minute foundation. Reviewer can catch errors immediately rather than discovering them at the end.

---

## Minimum Search Requirements

### Recognition Events (Dimension 3)
**Minimum time**: 2.5 hours of searching

**Required searches**:
- Governor's office website and press releases
- State HR department recognition programs
- Department of Administration awards
- Major agency websites (top 5 by employment)
- Legislative proclamations
- News coverage of state employee events

**Why it matters**: North Carolina initially found zero recognition events because searching stopped too early. Extended search found multiple programs and events, raising their score significantly.

---

### Training Budget (Dimension 4)
**Minimum time**: 2 hours of searching

**Required locations**:
- State budget appropriations (line items for "training" or "professional development")
- HR department annual reports
- Individual agency budget documents
- Legislative fiscal notes

**If truly not published**: Score = 0 for this component, flagged as "DATA NOT PUBLISHED"

**Why it matters**: We don't estimate or extrapolate missing data. Scoring zero creates incentive for transparency rather than rewarding opacity.

---

## Data Quality Transparency

Every data point in every state report carries one of three flags:

**✅ Verified** – Direct from authoritative government source, confirmed accurate  
**⚠️ Estimated** – Calculated from partial data using documented methodology  
**❌ Data Not Published** – Could not be found despite extensive searching

**Example from Virginia**:
- Salary competitiveness: ✅ Verified (Virginia DataPoint database)
- Employer health premium contribution: ⚠️ Estimated (88-98% from contract documents)
- Training budget: ❌ Data Not Published (zero consolidated figure found)

**Why it matters**: Users deserve to know our confidence level in every finding. Transparency about limitations builds credibility.

---

## Our Track Record

Across five states assessed with framework v2.2:

**Formula Compliance**: 100% ✅  
Every state uses identical formulas. Zero unauthorized modifications.

**Data Accuracy**: Zero major errors after checkpoints implemented ✅  
Reality checks caught salary errors in Massachusetts and Washington before they propagated.

**Methodology Consistency**: 100% ✅  
All five states are directly comparable using identical methodology.

**Source Documentation**: 100% ✅  
Every data point has URL, date, and methodology notes.

---

## Continuous Improvement

Quality control isn't static—it evolves based on lessons learned:

**v1.0 → v2.0**: Added data quality flags and transparency standards  
**v2.0 → v2.1**: Added formula lock and minimum search times  
**v2.1 → v2.2**: Added reality checks and approval checkpoints

Each improvement came from actual errors we discovered and corrected. Future versions will address any new challenges that emerge.

---

## For Deeper Detail

This summary covers the essential quality controls. For complete documentation:

**[Full Quality Control Procedures](link-to-full-doc)**: Every checklist, reality check range, and verification step documented in detail

**[Framework Change History](link-to-full-doc)**: How quality controls evolved through testing across five states

**[State Reports](link-to-reports)**: See quality controls in action—every report shows data quality flags and source documentation

---

## Why This Matters

These quality controls mean you can trust PSAI scores:
- States are compared using identical, verified methodology
- Data errors are caught early through systematic checks
- Missing data is acknowledged openly rather than hidden
- Every finding is traceable to authoritative sources
- The methodology is transparent, replicable, and continuously improving

---

*Last updated: December 31, 2025 | Framework version: 2.2*
