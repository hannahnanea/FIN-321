# Stage 5 – Final Analysis & Recommendation

**Course:** FIN-321  
**Student:** Hannah Sheveland  
**Deliverable:** Executive FX Hedge Recommendation Memo  

---

## A. Exposure Summary

The firm is exposed to foreign exchange risk through a **€3,879,310 EUR receivable** due in **one year**. Because the firm’s functional currency is **USD**, fluctuations in the EUR/USD exchange rate directly affect the dollar value of this incoming cash flow. A depreciation of the euro would reduce USD proceeds and negatively impact cash flow, budgeting accuracy, and reported financial performance.

As a result, Treasury must evaluate hedging strategies that stabilize USD cash flows while balancing cost, flexibility, and opportunity for upside.

---

## B. Summary of Hedge Outcomes

Three hedging strategies were evaluated using the Stage 4 Excel model: **forward hedge, money market hedge, and EUR put option**.

- **Forward Hedge:** Locks in a fixed USD conversion rate of 1.0875 USD/EUR. This strategy delivers **certain and predictable USD proceeds**, fully eliminating FX risk.

- **Money Market Hedge:** Replicates the forward contract using spot conversion and interest rate differentials between USD and EUR. The model confirms that **money market proceeds closely match forward proceeds**, validating interest rate parity.

- **Option Hedge (EUR Put):** Provides downside protection through a strike price of 1.16 USD/EUR while allowing upside participation if the euro appreciates. However, this flexibility comes at a **known upfront premium cost**, which reduces net proceeds when the euro remains stable or strengthens moderately.

Across all scenarios, the forward and money market hedges deliver nearly identical outcomes, while the option hedge introduces asymmetry—limited downside with retained upside.

---

## C. Sensitivity Interpretation

The ±5% sensitivity analysis around the spot rate highlights clear behavioral differences:

- **EUR Depreciation:**  
  The forward and money market hedges fully protect against downside, producing stable USD proceeds regardless of spot movements. The option hedge also protects against depreciation but results in lower net proceeds due to the premium paid.

- **EUR Appreciation:**  
  The forward and money market hedges forgo upside, as proceeds are fixed. The option hedge benefits from euro appreciation, allowing USD proceeds to increase once spot exceeds the strike price, partially offsetting the premium cost.

Overall, the analysis illustrates the classic trade-off between **certainty (forwards/MM)** and **flexibility (options)**.

---

## D. Strategic Recommendation

**Recommended Strategy: Forward Hedge**

Given the firm’s objective of protecting a known cash inflow and ensuring budget certainty, the **forward hedge** is the most appropriate strategy.

The forward hedge:
- Eliminates FX risk entirely
- Provides predictable USD cash flows
- Requires no upfront premium
- Aligns with conservative treasury risk management practices

The money market hedge is economically equivalent but operationally more complex, while the option hedge introduces unnecessary cost for upside that is not essential to the firm’s objectives.

---

## E. Executive Justification

From a management perspective, the forward hedge best supports:

- **Cash flow stability:** Guaranteed USD proceeds improve planning and liquidity management.
- **Budget certainty:** Eliminates forecast volatility caused by FX movements.
- **Simplicity & control:** Fewer transactions and lower operational risk than synthetic hedges.
- **Cost efficiency:** Avoids option premiums that reduce expected value.

If hedge accounting were applied, the forward hedge would also be easier to document and test for effectiveness, reinforcing governance and audit readiness.

---

## Extra Credit – Areas for Further Study & Improvement

### 1. Claude Skills (Automation & Live Data Integration)

Claude Skills could automate the model by pulling **live FX spot rates, forward curves, and interest rates**, updating the Excel file automatically, and regenerating hedge recommendations in real time. This would transform the model from a static analysis into a dynamic treasury decision tool.

---

### 2. OpenAI Codex / Code Interpreter

Codex could convert the Excel hedge logic into **Python-based analytics**, enabling Monte Carlo simulations, stress testing, and probabilistic outcome analysis. This reduces operational risk by allowing models to be regenerated and validated programmatically.

---

### 3. Claude Code / Multi-File Reasoning

Multi-file reasoning would allow an AI system to read and maintain consistency across **specifications (Stage 2), Excel models (Stage 3–4), and written recommendations (Stage 5)**. This ensures alignment between logic, implementation, and communication.

---

### 4. GitHub Automation & Version Control

Version control ensures every change to hedge specifications, spreadsheets, and AI prompts is recorded and reversible. In finance, this is critical for:

- Auditability and internal controls
- Hedge documentation and effectiveness testing
- Multi-analyst collaboration
- Error prevention and transparency

By storing Stages 2–4 in GitHub, the hedge model becomes **reproducible, reviewable, and governance-ready**, mirroring professional treasury workflows.

---

### 5. Accounting & Audit Integration

Reproducible, version-controlled hedge models support hedge accounting by:
- Providing clear documentation of hedge intent
- Demonstrating effectiveness over time
- Serving as audit evidence for OCI vs. P&L treatment

GitHub-backed models significantly reduce audit friction and improve confidence in reported results.

---

## Closing Perspective

This project demonstrates the full lifecycle of modern financial analysis: **specification → modeling → AI prompting → automation → executive decision-making**. The skills developed mirror real-world workflows used in corporate treasury, investment banking, FP&A, audit, and AI-driven analytics roles, making this a portfolio-ready artifact for professional use.

