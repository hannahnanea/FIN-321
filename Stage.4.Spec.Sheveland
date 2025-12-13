# GOAL
Create a complete, professional Excel (.xlsx) spreadsheet that models FX hedging strategies for a **EUR receivable** using a **forward contract, money market hedge, and option hedge**, fully aligned with FIN-321 Stage 2 and Stage 3 specifications.

The output must be a **downloadable Excel file** suitable for Treasury / CFO review, with transparent logic, auditability, and academic rigor.

---

# CONTEXT
You are acting as a **Financial Modeling Assistant** supporting a Treasury Analyst. This model is part of a staged analytical pipeline:
- **Stage 2** defined the economic logic and hedge valuation workflow
- **Stage 3** implemented preliminary Excel structure
- **Stage 4 (this task)** converts that logic into a fully executable AI-driven spreadsheet build

Functional currency: **USD**  
Exposure type: **Known EUR receivable**  
Hedge horizon: **1 year**

---

# INPUT VARIABLES (ALL VALUES EXPLICIT)
Use **only** the following values. Do not infer or substitute.

- `FC_AMT` = **3,879,310** (EUR receivable)
- `S0_in` = **1.16** USD/EUR (spot rate at inception)
- `F0_in` = **1.0875** USD/EUR (1Y forward rate)
- `R_USD` = **3.42%** annual (USD interest rate)
- `R_FC` = **2.15%** annual (EUR interest rate)
- `K_PUT` = **1.16** USD/EUR
- `K_CALL` = **1.16** USD/EUR
- `PREM_PUT` = **0.015** USD per EUR
- `PREM_CALL` = **0.018** USD per EUR
- `T_DAYS` = **360**
- `T_YRS` = `T_DAYS / 360`

Scenario exchange rates (`S_T`) must span **±5% around spot**:
- From `0.95 × S0_in` to `1.05 × S0_in`

---

# SPREADSHEET REQUIREMENTS
Generate **one Excel workbook** with clean layout and labeled sections.

## REQUIRED MODEL SECTIONS
1. Inputs & Assumptions
2. Unhedged Benchmark
3. Forward Hedge
4. Money Market Hedge (3-step)
5. Option Hedge (Put & Call logic)
6. Sensitivity Analysis (±5%)
7. Outputs & KPIs

---

# NAMED RANGE DEFINITIONS (MANDATORY)
All inputs must be defined as **Excel Named Ranges** using *exact* names below:

- `FC_AMT`
- `S0_in`
- `F0_in`
- `R_USD`
- `R_FC`
- `K_PUT`
- `K_CALL`
- `PREM_PUT`
- `PREM_CALL`
- `T_DAYS`
- `T_YRS`

No alternative naming conventions are permitted.

---

# MODEL LOGIC (PSEUDOCODE)

## Unhedged
```
USD_Unhedged = FC_AMT × S_T
```

## Forward Hedge
```
USD_Forward = FC_AMT × F0_in
```

## Money Market Hedge (Parity Check Required)
```
PV_EUR = FC_AMT / (1 + R_FC × T_YRS)
USD_PV = PV_EUR × S0_in
USD_MMH = USD_PV × (1 + R_USD × T_YRS)
```

## Option Hedge (EUR Put)
```
Premium_Cost = FC_AMT × PREM_PUT

If S_T < K_PUT:
    Payoff = (K_PUT − S_T) × FC_AMT
Else:
    Payoff = 0

USD_Option = (FC_AMT × S_T) + Payoff − Premium_Cost
```

---

# SENSITIVITY ANALYSIS
Create a scenario table where:
- Rows = exchange rates from `0.95 × S0_in` to `1.05 × S0_in`
- Columns include:
  - Unhedged
  - Forward
  - Money Market
  - Option

All values must update dynamically from named ranges.

---

# FORMATTING & COLOR CODING (STRICT)
Use Excel fill colors exactly as follows:
- **Yellow** → Input cells / decision variables
- **Blue** → Assumptions
- **Green** → Formula-driven cells
- **Gray** → Outputs, KPIs, results

Apply consistent fonts, borders, and section headers suitable for professional submission.

---

# OUTPUT REQUIREMENTS
The model must clearly display:
- USD proceeds under each hedge
- Minimum & maximum outcomes
- Downside protection vs unhedged
- Opportunity cost of hedging

Include clear labels and units for all outputs.

---

# VERIFICATION INSTRUCTIONS
You must:
1. **Validate interest rate parity** between Forward and Money Market hedges
2. Confirm **all named ranges exist and are correctly referenced**
3. Provide a **full formula map** (cell → formula) for auditability
4. Flag any inconsistencies or broken links

---

# EXPORT
Return:
- A **fully functional downloadable `.xlsx` file**
- Confirmation that all requirements above were met

Do not include explanations outside the spreadsheet unless explicitly requested.

---

# END OF PROMPT

