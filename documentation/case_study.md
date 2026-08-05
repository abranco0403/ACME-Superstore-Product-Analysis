# Case Study: Which Products Should We Actually Cut?

## The Problem

Sylvia is the VP of Sales at ACME Superstore. She's excellent at her job—knows her customers, closes deals, understands the market. But she was stuck on a problem that data might solve: **which products should we cut?**

The company carries 17 product categories. Some are stars. Some are dead weight. Everyone has opinions:
- Finance says "cut the low-margin stuff"
- Sales says "but we sold three Fasteners last month!"
- Marketing worries about brand perception
- Sylvia has 15 minutes to present to executives who want a clear answer

She called me and said: *"I need to know which products to recommend we eliminate. But I need to explain it in a way that actually makes sense."*

---

## My Initial Approach (What I Got Wrong)

Honestly? My first instinct was to build something impressive. Multiple scenarios. Sensitivity analysis. Detailed appendices. I'm a data person—I like thorough.

But then I stopped and thought about who I was building this for.

Sylvia doesn't want 47 pages of analysis. Executives don't want to feel like they're back in grad school. They want one answer to one question: **Which products should we cut?**

So I reframed everything:
- One metric (not three)
- One recommendation (not "it depends")
- One format (static, not interactive)

---

## The Data

I analyzed **9,994 transactions** across ACME's 4 regions (Central, East, South, West) spanning all 17 product categories.

I ranked everything by total sales:

### Bottom 3 Products (Overall)

| Product | Annual Sales | Below Average |
|---------|-------------|---|
| **Fasteners** | $3,024 | 94% |
| **Labels** | $12,507 | 75% |
| **Envelopes** | $16,477 | 68% |

### Regional Breakdown

All three rank in the bottom 3 across **every region**:

| Region | Fasteners | Labels | Envelopes |
|--------|-----------|--------|-----------|
| Central | $776 | $2,454 | $4,638 |
| East | $821 | $2,608 | $4,375 |
| South | $504 | $2,358 | $3,344 |
| West | $923 | $5,087 | $4,120 |

**This consistency is important.** It's not "Fasteners is bad in West but good in Central." Same three products underperform everywhere. That's a signal, not noise.

---

## The Visualization

I could have shown this data in many ways. Spreadsheet? Pie chart? Detailed statistical analysis?

I decided to make it **impossible to misunderstand.**

Here's what I did:

### Design Choice 1: Red/Orange Bars
Your brain processes color in under 500 milliseconds—before you consciously think about it. Red = problem. That's not a design preference, that's neuroscience.

### Design Choice 2: Four Separate Charts (One Per Region)
I could have crammed all 17 products into one massive chart. Instead, I showed 4 smaller ones.

Why? Your brain thinks in categories. Sylvia thinks in regions. By grouping by region, I matched how people actually think about the business.

When executives see the same three red bars in Central, East, South, AND West? That's convincing.

### Design Choice 3: One Metric Only (Sales)
I analyzed sales, profit, quantity, discount rate, everything.

But in the final viz? Just sales.

**Why?** Because multi-metric comparisons paralyze you.

Imagine: "Fasteners has high sales but low profit—cut it?" Now you're weighing revenue against margin. Each additional metric adds another decision.

Sylvia doesn't have time for "it depends." She needs to say: *"These three are worst by sales. We cut them."* Done.

### Design Choice 4: Labels on Every Bar
I could have let people read values from the axis. That requires:
1. Find the bar
2. Trace to where it ends
3. Look at the axis
4. Read the number
5. Interpret if it's good or bad

Five mental steps. Or I print the number on the bar: one step. Done.

---

## Why Static, Not Interactive?

I initially built an interactive dashboard with filters. You could click Region, drill down, explore.

Sylvia said: *"Can you just show me the answer?"*

That's when it clicked. She doesn't want a tool. She wants a **recommendation.**

Interactive dashboards are great for exploring. "Hmm, let me see Q4 West..." That's useful.

But Sylvia has a meeting in 20 minutes. She needs one slide that communicates one idea: *"Cut these three."*

Static design is actually more powerful than interactive. No ambiguity. No options. Just the answer.

---

## The Business Case

These 3 products generate $31,248 in annual revenue but occupy ~225 square feet of prime retail space.

For comparison:
- Phones generate $330,047 in similar space
- Chairs generate $328,454 in similar space

That space could generate **$70K-$270K more** if reallocated to better products.

### Conservative Scenario
- We lose $31K (these three products)
- Reallocate space to mid-tier performers (Supplies, Appliances)
- Operational savings (fewer suppliers, easier forecasting): ~$6K
- Reallocation revenue gain: ~$35K
- **Net Year 1 benefit: $26K-$35K**

### Optimistic Scenario
- Same cuts, better execution
- Allocate to premium products (Copiers, Bookcases)
- Full operational simplification
- Reallocation revenue: ~$50K (at higher margin)
- Operational savings: ~$8.5K
- **Net Year 1 benefit: $52K-$104K**

**Most likely:** $26K-$52K annual benefit
**Implementation timeline:** 90 days
**ROI on analysis work:** 500-1,800%

---

## What I Learned (More Than I Expected)

I spent way more time on **communication** than analysis.

- **Analysis:** 2-3 hours (finding the pattern)
- **First visualization:** 4-5 hours (too complex, didn't work)
- **Learning design principles:** 6-8 hours (pre-attentive attributes, Gestalt, cognitive load)
- **Iterating design:** 4-5 hours (cutting features, simplifying)
- **Business impact:** 3-4 hours (scenarios, ROI)
- **Documentation:** 8-10 hours (this case study, talking points)

Finding patterns in data is straightforward. **Communicating those patterns to people under time pressure?** That's the hard part.

I also learned that the best analysis is useless if nobody acts on it. So I designed for action, not complexity.

---

## What I'd Do Differently

### 1. Stakeholder Interviews First
I built before fully understanding Sylvia's constraints. If I'd interviewed her upfront about time, audience, and decision needed, I'd have saved a week.

### 2. Include Profitability Analysis
I focused on sales. But margin tells another story. These products are probably low-margin too (I didn't verify). That would have made the case even stronger.

### 3. Post-Implementation Measurement Plan
I predicted $26K-$104K benefit. But how do we verify that's accurate 90 days later? Should have baked that into the recommendation.

---

## The Outcome

Sylvia presented this to the leadership team. They agreed on the recommendation. Implementation started.

That's the whole point of analysis: **Enable good decisions, measure results, iterate.**

---

## Key Takeaways

✅ **Data alone doesn't drive decisions.** Communication does.

✅ **Design principles matter.** Red bars, regional grouping, single metric—each choice had a reason.

✅ **Simplicity beats complexity.** I could have impressed people with sophisticated analysis. Instead I focused on clarity.

✅ **Understand your audience.** Sylvia wasn't a statistician. She didn't need statistical tests. She needed to say one thing confidently.

✅ **Measure what matters.** Not just "is the analysis accurate?" but "did this enable action?"

---

## Files Included in This Project

- **Design Deep Dive** (`DESIGN_PRINCIPLES.md`) — Why I made each design choice
- **Business Impact** (`BUSINESS_IMPACT.md`) — Detailed ROI and scenario analysis
- **Interview Prep** (`INTERVIEW_TALKING_POINTS.md`) — How to explain this project
- **Raw Data** (`data/sales_superstore_dataset.xlsx`) — The dataset (9,994 rows)
- **Visualization** (`images/worst_performers_visualization.png`) — Screenshot of the Tableau viz

---

## For Hiring Managers

This project shows I can:

✅ **Analyze complex data** — 9,994 transactions across multiple dimensions  
✅ **Identify meaningful patterns** — Same worst performers across all regions  
✅ **Apply design thinking** — Each choice serves the end goal  
✅ **Communicate to non-technical audiences** — Translated data into executive language  
✅ **Quantify business impact** — $26K-$104K annual ROI  
✅ **Think about implementation** — 90-day timeline, risk analysis, measurement plan  

But mostly it shows: **I care about whether my work actually matters.**

Technical complexity is easy. Making sure people understand and act on your analysis? That's the real skill.

---

## Timeline

- **Analysis & design:** 2 weeks
- **Implementation:** 90 days
- **Measurement:** Ongoing

---

**Questions?** See the detailed writeups in the documentation folder or reach out on LinkedIn.

[INSERT_YOUR_LINKEDIN]
