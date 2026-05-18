# Main Analysis Tree: Why US Healthcare is Expensive

**Starting point:** Prices in the US are 5-10× higher than similar-quality countries (Mexico, Europe). Appendectomy: $25-60k US vs $3-8k Mexico. ICU: $10k/day US vs $1k/day Mexico.

**Core question:** If there's little regulation and costs are similar worldwide, why don't entrepreneurs open cheaper hospitals and capture the market?

This document follows a thought experiment: **You want to open a hospital with normal prices.** What stops you?

---

## The Thought Experiment: Opening a Cheaper Hospital

### Barrier 1: [Hospital Contracting Leverage](facts/1.1.4-contracting-leverage.md)
**What happens:** You open hospital with 40% lower prices. You approach insurance companies. Dominant hospital tells insurers: "Include them and we leave your network."

**Result:** Insurers reject you. Without insurance contracts, no patients. This practice is **legal** in the US. 90% of metro areas have one system controlling >50% of beds.

**Subcauses:**
- Why dominant hospitals have this power: [Geographic Captivity](facts/1.1.1-geographic-captivity.md) - Emergency patients need nearest hospital, giving local monopolies power

### Barrier 2: [Certificate of Need Laws](facts/1.6-certificate-of-need.md)
**What happens:** In 32 states, you need government approval to open a hospital. Must prove "community need." Existing hospitals can object and block you.

**Result:** Even if you have capital and plan, state board (often with hospital representatives) denies your application. Legal barrier to entry.

### Barrier 3: [Labor Costs 2-4× Higher](facts/1.4-labor-costs.md)
**What happens:** You try to hire nurses and doctors at competitive wages. US nurses cost $75-90k/year vs $25-35k Europe. Doctors $200-600k vs $70-150k Europe.

**Result:** Labor is 50-60% of hospital costs. Even with efficiency, you can only undercut by ~20%, not enough to disrupt market.

**Subcauses:**
- Why you can't hire foreign workers: [Immigration Barriers](facts/1.5-immigration-barriers.md) - Visa quotas, state licensing blocks foreign credentials

### Barrier 4: [EMTALA Forces Unprofitable Patient Mix](facts/1.3.3-emtala.md)
**What happens:** You want to specialize in profitable procedures (cataracts, elective surgery). Federal law requires emergency rooms to treat ALL patients regardless of ability to pay.

**Result:** Cannot cherry-pick profitable cases. Must cross-subsidize uncompensated care (~$40-50B/year across US hospitals). Your cost advantage disappears.

### Barrier 5: [Malpractice System Blocks Contracts](facts/1.9-malpractice-waivers.md)
**What happens:** You want to offer lower prices by negotiating reasonable liability caps via contract (like other countries). Malpractice insurance costs $30-80k/year per doctor.

**Result:** **Waivers are illegal in healthcare.** Courts will invalidate contracts limiting liability. Cannot reduce costs through contractual risk management. Must charge high prices to cover legal exposure.

---

## Secondary Factors (Not Direct Blockers, But Make It Worse)

### [Perverse Insurer Incentives (MLR)](facts/1.2.1-mlr-regulation.md)
Medical Loss Ratio regulation caps insurer profits at 15-20% of costs. Higher costs → higher absolute profit. Makes existing insurers lazy about negotiating.

**Why this doesn't block you directly:** You could theoretically create a new insurer with lower costs and capture market. But combined with Barrier 1 (contracting leverage), hospitals won't work with your insurer either. The 15-20% cap is reasonable - if you need more, you're inefficient or scamming customers.

### [Administrative Costs 3-5× Higher](facts/1.7-admin-overhead.md)
US spends 25-30% on billing/bureaucracy vs 5-8% Europe. Hundreds of insurers, thousands of billing codes, prior authorization complexity.

**Why this doesn't block you directly:** You can vertically integrate (create both hospital + insurer). Kaiser Permanente does this successfully with much lower admin costs. The fact that others don't reveals the real barriers are elsewhere.

---

## Common Misconceptions (Not Root Causes)

These factors seem like barriers but do NOT actually prevent competition:

### 1. EMTALA (must treat emergencies without guaranteed payment)
**Why it seems like a problem:** Federal law requires hospitals with ERs to treat all patients regardless of ability to pay.

**Why it's NOT a blocker:**
- Don't want emergencies? Don't build an ER (ambulatory surgery centers avoid this)
- If you DO have ER → 10-15% uncompensated care, but with 40% lower costs, still very profitable
- Insurance pays normal rates; huge margins even absorbing non-payment cases

### 2. Emergency patients can't compare prices
**Why it seems like a problem:** Heart attack victims can't shop around.

**Why it's NOT a blocker:**
- Insurers CAN negotiate prices in advance for all procedures
- Patient doesn't need to compare in the moment
- Real problem: [contracting leverage](facts/1.1.4-contracting-leverage.md) prevents insurers from negotiating effectively

### 3. High hospital construction costs
**Why it seems like a problem:** Building a hospital costs $100-500 million.

**Why it's NOT a blocker:**
- Same construction costs worldwide
- If Mexico has same capital costs but charges 5-10× less, while US charges 5-10× more
- US should have BETTER return on investment, not worse
- Doesn't explain why competition doesn't emerge

---

## Summary

**Five direct barriers prevent competition:**
1. ✅ Hospital contracting leverage (legal extortion)
2. ✅ Certificate of Need laws (government blocks entry)
3. ✅ Labor costs 2-4× higher (can't import workers)
4. ✅ EMTALA (must treat unprofitable patients)
5. ✅ Malpractice waivers illegal (can't manage legal costs)

**Two secondary factors make it worse:**
- ⚠️ MLR regulation - existing insurers don't fight costs
- ⚠️ Administrative overhead - adds 25-30% baseline cost (but can be bypassed via vertical integration)

**The system is trapped in a Nash equilibrium:**

No single actor can improve it unilaterally:
- **New hospital** → blocked by CON laws, contracting leverage, EMTALA, high labor costs
- **New insurer** → cannot force lower hospital prices (hospitals have leverage)
- **Patient** → no choice in emergencies, no price transparency
- **Government** → politically difficult to reform (powerful lobbies)

**The core problem:** We're spending hundreds of billions of dollars per year on lawyers, billing departments, lobbying, and fighting between hospitals, insurers, and patients - instead of simply curing people. We have the resources, technology, and professionals. What we lack is a system that allows competition to work.

**With proper reforms**, we could have the same medical procedures at a fraction of current costs, redirect that money to medical research, better salaries for healthcare workers, or return it to families. Instead, we burn it in a system designed to protect monopolies.

This creates a stable but expensive equilibrium that persists despite being 2-3× more costly than comparable nations.

---

## Supporting Resources

- **[examples.md](resources/examples.md)** - Concrete numerical examples (appendectomy: $33k US vs $5k Europe)
- **[comparisons.md](resources/comparisons.md)** - USA vs other developed nations data
- **[solutions.md](resources/solutions.md)** - Potential reforms that could break the equilibrium
