# Finance for Non-Finance Professionals — Quick Notes

A compact, no-fluff README that distills the four PDFs (Week 1–4) into **key learnings**, **must-know formulas**, and **practical tips**.

> Source decks: `week1.pdf`, `week2.pdf`, `week3.pdf`, `week4.pdf`

---

## Table of Contents
- [Week 1 — Valuation & Discounting](#week-1--valuation--discounting)
- [Week 2 — Capital Budgeting (How to Spend Money)](#week-2--capital-budgeting-how-to-spend-money)
- [Week 3 — Measuring Cash Creation & Flow](#week-3--measuring-cash-creation--flow)
- [Week 4 — Cost of Capital](#week-4--cost-of-capital)
- [Formula Glossary (One-Pager)](#formula-glossary-onepager)
- [Mini Worked Examples](#mini-worked-examples)
- [Study Tips](#study-tips)

---

## Week 1 — Valuation & Discounting

### Big Ideas
- **Time value of money**: ₹1 today > ₹1 tomorrow.
- **Compounding** grows value forward; **discounting** brings future rupees back to today.
- **DCF** (discounted cash flow) is the bedrock of valuation (bonds, stocks, real estate, M&A).
- **Comps** (relative valuation) are quick but can mislead if comparability is weak.

### Formulas
- **Future Value (FV)**  
  `FV = PV × (1 + r)^t`
- **Present Value (PV)**  
  `PV = FV / (1 + r)^t`
- **Annualized Return (solve r)**  
  `r = (FV / PV)^(1/t) − 1`
- **General DCF Valuation**  
  `Value = Σ [ CF_t / (1 + r)^t ]`
- **Comps (price by attribute)**  
  `Price_target = (Price/Attribute)_comp × Attribute_target`

---

## Week 2 — Capital Budgeting (How to Spend Money)

### Big Ideas
- **NPV** is the gold standard (objective, risk & timing aware).
- **IRR** is intuitive but can mislead (scale, timing, multiple/no IRRs).
- **Payback** is quick but ignores cash after cutoff and risk.
- Ratios (ROIC, ROA, ROE, margins) are helpful context, not decision rules.
- Always do **sensitivity/scenario analysis**—forecasts are uncertain.

### Formulas
- **Net Present Value (NPV)**  
  `NPV = Σ [ CF_t / (1 + r)^t ] − Initial_Investment`  
  _Accept if `NPV > 0`._
- **Internal Rate of Return (IRR)**  
  Rate `r*` such that `NPV(r*) = 0`.  
  _Accept if `IRR > hurdle rate`._
- **Payback Period**  
  Time until cumulative **undiscounted** cash inflows = initial outlay.
- **ROIC (Return on Invested Capital)**  
  `ROIC = NOPAT / Invested_Capital`

---

## Week 3 — Measuring Cash Creation & Flow

### Big Ideas
- **Cash is king** → Value follows **free cash flow (FCF)**, not accounting earnings.
- **Working capital** ties up cash; increases are a **cash drain**.
- **Depreciation** is non-cash (add back); **CAPEX** is real cash out.
- Include **salvage/terminal value** at project end; **taxes** are real cash flows.

### Formulas
- **Working Capital (WC)**  
  `WC = Current Assets − Current Liabilities`  
  ΔWC > 0 → cash **outflow**; ΔWC < 0 → cash **inflow**.
- **Free Cash Flow (core form)**  
  `FCF = Operating Profit (after tax) − ΔWC + Depreciation − CAPEX + After-tax Salvage`

---

## Week 4 — Cost of Capital

### Big Ideas
- **Capital structure** = mix of **Debt** (cheaper, tax shield) and **Equity** (residual risk/return).
- **Risk-free rate** (Treasuries) is the floor; risky assets add **risk premiums**.
- **Beta** measures exposure to market risk; use **CAPM** for cost of equity.
- Combine into **WACC** to discount project/firm cash flows (use project-appropriate rates).

### Formulas
- **CAPM (Cost of Equity, Re)**  
  `Re = Rf + β × (Equity_Premium)`
- **After-Tax Cost of Debt, Rd**  
  `Rd_after = Rd_pre × (1 − tc)`
- **WACC**  
  `WACC = (E/(D+E)) × Re + (D/(D+E)) × Rd_after`

---

## Formula Glossary (One-Pager)

```text
FV = PV × (1 + r)^t
PV = FV / (1 + r)^t
r = (FV/PV)^(1/t) − 1
Value (DCF) = Σ[ CF_t / (1 + r)^t ]

NPV = Σ[ CF_t / (1 + r)^t ] − Initial
IRR: r* s.t. NPV(r*) = 0
Payback: years to recover initial (undiscounted)
ROIC = NOPAT / Invested Capital

WC = CA − CL
ΔWC: + is cash outflow, − is cash inflow
FCF = NOPAT − ΔWC + Dep − CAPEX + After-tax Salvage

Re = Rf + β × (Equity Premium)
Rd_after = Rd_pre × (1 − tc)
WACC = (E/(D+E))Re + (D/(D+E))Rd_after

---

## Mini Worked Examples

**1) FV / PV**

* Deposit ₹1,000 at 11% for 5 years:
  `FV = 1000 × 1.11^5 ≈ ₹1,685.06`
* Value today of ₹175 in 5 years at 4%:
  `PV = 175 / 1.04^5 ≈ ₹143.84`

**2) NPV (10% discount rate)**

* CF₀ = −1,500; CF₁ = 900; CF₂ = 750
  `NPV = −1500 + 900/1.1 + 750/1.1^2 ≈ −₹61.98`

**3) FCF (simple)**

```
NOPAT = 70
ΔWC = +50 (cash outflow)
Dep = 100
CAPEX = 0
Salvage(after-tax) = 0
FCF = 70 − 50 + 100 − 0 + 0 = 120
```

**4) CAPM & WACC**

```
Rf = 3%, Equity Premium = 5.5%, β = 1.2
Re = 3% + 1.2×5.5% = 9.6%

Pre-tax Rd = 6%, tc = 25% ⇒ Rd_after = 4.5%
E = 600, D = 400 ⇒ weights: E=60%, D=40%
WACC = 0.6×9.6% + 0.4×4.5% = 7.56%
```

---

## Study Tips

* **Always map cash flows**: amount + timing → discount with the **right rate**.
* **Sanity check IRR vs NPV** (especially with sign changes, different scales, or odd timing).
* **Track ΔWC, Dep, CAPEX, Taxes, Salvage** explicitly in your FCF build.
* Use **WACC** for average risk projects; adjust discount rate for project-specific risk.

---

### Attribution

Summarized from course slides:

* `week1.pdf` — Valuation & Discounting
* `week2.pdf` — Capital Budgeting
* `week3.pdf` — Cash Creation & FCF
* `week4.pdf` — Cost of Capital

```
```
