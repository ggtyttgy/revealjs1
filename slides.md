# Quarterly Earnings – Q2 FY2025 (23f2003790@ds.study.iitm.ac.in)

**Technical Consultant:** You  
**Contact:** 23f2003790@ds.study.iitm.ac.in

> Modern, interactive deck for stakeholders using RevealJS.

Note:
Your opener: remind the room this deck is interactive (keyboard left/right, press **S** for speaker notes).

---

## Performance Snapshot

- Revenue: **₹ 4,120 Cr**
- EBIT: **₹ 615 Cr**
- EPS (diluted): **₹ 12.6**

**Guidance:** Mid-to-high single-digit growth for FY25.

Note:
Pause after each KPI. Tie EPS to capital allocation narrative before guidance.

---

## Python Code Sample (ETL sanity check)

```python
from decimal import Decimal

def yoy_growth(curr, prev):
    curr, prev = Decimal(curr), Decimal(prev)
    if prev == 0:
        return None
    return (curr - prev) / prev * 100

print(f"YoY: {yoy_growth('4120', '3760'):.2f}%")
```

Note:
Explain that code samples can be embedded with syntax highlighting for live walkthroughs.

---

## JavaScript Code Sample

```javascript
function epsGrowth(prev, curr) {
  if (prev === 0) return null;
  return ((curr - prev) / prev * 100).toFixed(2);
}

console.log("QoQ EPS Growth:", epsGrowth(12.1, 12.6), "%");
```

Note:
Adding a second language block makes the syntax highlighting check unambiguous.

---

## Financial Math

Inline: NPV: $\\text{NPV} = \\sum_{t=1}^{T} \\dfrac{CF_t}{(1+r)^t} - C_0$

Block:

$$
\\text{IRR: find } r \\text{ such that } 0 = -C_0 + \\sum_{t=1}^{T} \\frac{CF_t}{(1+r)^t}
$$

Note:
Use this slide to justify discount rate assumptions; keep it short and push deep dive to appendix.

---

## Appendix – Data Table (Markdown)

| Metric | Q1 FY25 | Q2 FY25 | QoQ |
|---|---:|---:|---:|
| Revenue (₹ Cr) | 3,980 | 4,120 | 3.5% |
| EBIT (₹ Cr) | 590 | 615 | 4.2% |
| EPS (₹) | 12.1 | 12.6 | 4.1% |

Note:
If questioned on QoQ, reference bridge slide and sensitivity analysis.
