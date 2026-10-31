# Cross-Unit Formulas & Calculations: The EXIM Mathematical Toolkit

**Course:** MGN902: Export Import Procedure and Documentation  
**Scope:** Units I, II, and III  
**Pedagogical Objective:** Master every mathematical conversion, pricing formula, tax refund rule, finance calculation, and insurance adjustment tested in university numerical problems with full, step-by-step worked solutions.

---

## 1. Export Price Quotation & Incoterms Conversions

### A. Core Mathematical Structure
In international trade, prices build sequentially from the factory floor to the buyer's warehouse:

$$\text{Ex-Factory Price} = \text{Manufacturing Cost} + \text{Export Packaging} + \text{Factory Overhead} + \text{Profit Margin}$$

$$\text{FAS Price} = \text{Ex-Factory Price} + \text{Inland Transport to Port} + \text{CFS Handling} + \text{Port Entry Charges}$$

$$\text{FOB Price} = \text{FAS Price} + \text{Customs Clearance Charges} + \text{Stevedoring (Loading on Board)}$$

$$\text{CFR Price} = \text{FOB Price} + \text{Ocean Freight}$$

### B. The Definitive FOB-to-CIF Conversion Formula
Under standard commercial practice and Incoterms 2020, cargo insurance is contracted for **110% of the CIF value** (100% invoice value + 10% imaginary profit).

Therefore:
$$\text{CIF} = \text{CFR} + \text{Marine Insurance Premium}$$
$$\text{Marine Insurance Premium} = \text{Insurance Rate } (r) \times 1.10 \times \text{CIF}$$
$$\text{CIF} = \text{CFR} + [1.10 \times r \times \text{CIF}]$$
$$\text{CIF} - [1.10 \times r \times \text{CIF}] = \text{CFR}$$
$$\text{CIF} \times [1 - (1.10 \times r)] = \text{CFR}$$

$$\mathbf{CIF = \frac{FOB + \text{Ocean Freight}}{1 - (1.10 \times r)}}$$

*Where $r$ is the marine cargo insurance premium rate expressed as a decimal (e.g., 0.5% = 0.005).*

---

### Worked Problem 1: Full FOB to CIF Quotation
**Question:**  
An Indian exporter in Tirupur manufactures 5,000 cotton polo shirts. The cost and logistical expenses are:
- Ex-factory production cost: ₹200 per shirt
- Domestic transport from Tirupur to Chennai seaport: ₹25,000 (total)
- Port handling, palletization, and customs documentation: ₹15,000 (total)
- Loading charges onto ocean vessel (stevedoring): ₹10,000 (total)
- Ocean freight to Rotterdam: USD 2,500
- Marine cargo insurance premium rate: 0.6% on 110% of CIF value
- Target profit margin: 20% on ex-factory cost
- Applicable exchange rate: 1 USD = ₹83.00

*Calculate: (a) Ex-factory price, (b) FOB price in INR and USD, and (c) CIF price in USD.*

**Step-by-Step Solution:**

1. **Calculate Total Ex-Factory Price:**
   $$\text{Production Cost} = 5,000 \times ₹200 = ₹10,00,000$$
   $$\text{Profit Margin (20\%)} = 0.20 \times ₹10,00,000 = ₹2,00,000$$
   $$\text{Ex-Factory Price} = ₹10,00,000 + ₹2,00,000 = ₹12,00,000$$

2. **Calculate FOB Price in INR and USD:**
   $$\text{FOB Price (INR)} = \text{Ex-Factory} + \text{Inland Transport} + \text{Port Handling} + \text{Loading}$$
   $$\text{FOB Price (INR)} = ₹12,00,000 + ₹25,000 + ₹15,000 + ₹10,000 = ₹12,50,000$$
   $$\text{FOB Price (USD)} = \frac{₹12,50,000}{83.00} = \mathbf{USD\ 15,060.24}$$

3. **Calculate CIF Price in USD:**
   $$\text{Ocean Freight} = \text{USD } 2,500$$
   $$\text{Insurance Rate } (r) = 0.6\% = 0.006$$
   $$\text{CFR Value} = \text{FOB} + \text{Freight} = 15,060.24 + 2,500 = \text{USD } 17,560.24$$
   $$\text{CIF} = \frac{\text{CFR}}{1 - (1.10 \times 0.006)} = \frac{17,560.24}{1 - 0.0066} = \frac{17,560.24}{0.9934} = \mathbf{USD\ 17,676.91}$$

4. **Verification / Insurance Breakdown:**
   $$\text{Insured Value (110\% of CIF)} = 1.10 \times 17,676.91 = \text{USD } 19,444.60$$
   $$\text{Insurance Premium Paid} = 0.006 \times 19,444.60 = \text{USD } 116.67$$
   $$\text{Recomputed CIF} = \text{CFR } (17,560.24) + \text{Insurance } (116.67) = \mathbf{USD\ 17,676.91}\quad\checkmark$$

---

## 2. Duty Drawback Calculations

### A. Statutory Provisions
- **Section 74 of Customs Act, 1962 (Re-export of Imported Goods):**
  - If goods are re-exported in the exact same state without use: **98% of import duty paid** is refunded as drawback.
  - If goods were used after importation before re-export, drawback is reduced according to length of use:
    - *Up to 3 months:* 95%
    - *3 to 6 months:* 85%
    - *6 to 9 months:* 75%
    - *9 to 12 months:* 70%
    - *12 to 15 months:* 65%
    - *15 to 18 months:* 60%
    - *Exceeding 18 months:* 0% (Nil)
- **Section 75 of Customs Act, 1962 (Manufactured Exports):**
  - Granted under **All Industry Rates (AIR)** as a fixed percentage of the FOB value, subject to a statutory monetary cap per unit.

---

### Worked Problem 2: Duty Drawback Calculations
**Question:**  
(a) An electronics firm in Bengaluru imported testing instruments on 10 January 2026, paying basic customs duty of ₹5,00,000. After testing for 5 months, the equipment is re-exported to Germany on 20 June 2026. Calculate the admissible drawback under Section 74.  
(b) A garment exporter ships 10,000 cotton shirts at an FOB value of USD 10 each (Exchange rate: USD 1 = ₹83.00). The All Industry Rate (AIR) of Duty Drawback for this tariff line is 2.5% of FOB value, subject to a maximum cap of ₹22.00 per shirt. Calculate the total drawback receivable.

**Solution:**

**(a) Section 74 Drawback:**
- Period of use between import (10 Jan) and re-export (20 June) = 5 months and 10 days.
- Under statutory rules for use between 3 and 6 months, the admissible drawback rate is **85%**.
$$\text{Admissible Drawback} = 85\% \times ₹5,00,000 = \mathbf{₹4,25,000}$$

**(b) Section 75 Drawback:**
- Total FOB Value in INR:
  $$\text{FOB Value} = 10,000 \times 10 \times 83.00 = ₹83,00,000$$
- Uncapped Drawback at 2.5%:
  $$\text{Drawback at 2.5\%} = 0.025 \times ₹83,00,000 = ₹2,07,500\quad (\text{i.e., } ₹20.75 \text{ per shirt})$$
- Verify against Statutory Cap:
  $$\text{Statutory Maximum Cap} = 10,000 \times ₹22.00 = ₹2,20,000$$
- Since the calculated drawback per shirt (₹20.75) is lower than the cap (₹22.00), the exporter receives the full calculated amount:
  $$\mathbf{\text{Total Drawback Receivable} = ₹2,07,500}$$

---

## 3. GST Refund Mechanics for Zero-Rated Exports

Under **Section 16 of the IGST Act, 2017**, exports are zero-rated supplies. Exporters have two distinct mathematical routes:

### Route A: Export under LUT (Refund of Unutilized Input Tax Credit)
Governed by Rule 89(4) of the CGST Rules, 2017:

$$\mathbf{\text{Maximum Refund Amount} = \frac{\text{Turnover of Zero-Rated Supply of Goods and Services} \times \text{Net ITC}}{\text{Adjusted Total Turnover}}}$$

*Where:*
- *Turnover of Zero-Rated Supply:* Value of goods exported under LUT (capped at 1.5 times the domestic market value of like goods).
- *Net ITC:* Input Tax Credit availed on inputs and input services during the tax period (excluding capital goods).
- *Adjusted Total Turnover:* Total domestic turnover + export turnover during the period.

---

### Worked Problem 3: GST Refund under Rule 89(4)
**Question:**  
In July 2026, an export house records:
- Zero-rated export turnover under LUT: ₹60,00,000
- Domestic taxable turnover: ₹40,00,000
- Total Input Tax Credit (ITC) availed on raw materials/inputs: ₹9,00,000
- ITC availed on capital machinery purchased: ₹3,00,000 (excluded under Rule 89(4))
- Exempt domestic turnover: ₹10,00,000 (excluded from adjusted turnover)

*Calculate the maximum GST refund admissible to the exporter.*

**Solution:**
1. **Determine Net ITC:**
   $$\text{Net ITC (Inputs only)} = ₹9,00,000\quad (\text{Capital goods ITC is legally excluded})$$
2. **Determine Adjusted Total Turnover:**
   $$\text{Adjusted Total Turnover} = \text{Zero-Rated Turnover } (₹60,00,000) + \text{Domestic Taxable Turnover } (₹40,00,000) = ₹1,00,00,000$$
3. **Calculate Maximum Admissible Refund:**
   $$\text{Refund} = \frac{₹60,00,000 \times ₹9,00,000}{₹1,00,00,000} = 0.60 \times ₹9,00,000 = \mathbf{₹5,40,000}$$

---

## 4. Pre-Shipment Packing Credit Calculations

### A. Appraisal & Quantum Formula
$$\text{Eligible Quantum} = \text{FOB Value of Order} - \text{Exporter's Profit Margin}$$
$$\text{Maximum Bank Advance} = \text{Eligible Quantum} \times (1 - \text{Bank Margin Percentage})$$

### B. Interest Subvention Calculation (IES)
$$\text{Net Interest Rate Paid by Exporter} = \text{Bank Lending Rate} - \text{Government Subvention Rate (e.g., 3\% for MSME)}$$
$$\text{Total Interest Cost} = \text{Loan Amount} \times \left(\frac{\text{Net Interest Rate}}{100}\right) \times \left(\frac{\text{Tenure in Days}}{365}\right)$$

---

### Worked Problem 4: Packing Credit Appraisal & Interest
**Question:**  
An MSME leather exporter receives a confirmed export order worth USD 1,00,000.  
- Exchange rate: USD 1 = ₹83.00
- Exporter's estimated profit margin: 15% of FOB value
- Bank margin requirement: 20%
- Bank's base pre-shipment lending rate: 9.5% p.a.
- Government Interest Equalisation Scheme (IES) subvention: 3.0% p.a.
- Tenure: 120 days until shipment and liquidation via post-shipment bills.

*Calculate: (a) Sanctioned packing credit limit, (b) Net interest rate payable, and (c) Total interest cost saved due to IES.*

**Solution:**
1. **Calculate Order Value in INR:**
   $$\text{FOB Value} = 1,00,000 \times 83.00 = ₹83,00,000$$
2. **Calculate Eligible Quantum (Cost of Production):**
   $$\text{Profit Margin (15\%)} = 0.15 \times ₹83,00,000 = ₹12,45,000$$
   $$\text{Production Cost} = ₹83,00,000 - ₹12,45,000 = ₹70,55,000$$
3. **Calculate Sanctioned Packing Credit Advance (after 20% Bank Margin):**
   $$\text{Sanctioned Advance} = ₹70,55,000 \times (1 - 0.20) = ₹70,55,000 \times 0.80 = \mathbf{₹56,44,000}$$
4. **Calculate Net Interest Payable:**
   $$\text{Net Interest Rate} = 9.5\% - 3.0\% = \mathbf{6.5\%\ p.a.}$$
   $$\text{Interest Payable by Exporter} = ₹56,44,000 \times 0.065 \times \left(\frac{120}{365}\right) = \mathbf{₹1,20,611.51}$$
5. **Calculate Interest Saved via IES Subvention:**
   $$\text{Interest Subsidy Saved} = ₹56,44,000 \times 0.030 \times \left(\frac{120}{365}\right) = \mathbf{₹55,666.85}$$

---

## 5. Export Factoring Settlement Calculations

### A. Factoring Cash Flow Model
1. **Immediate Advance:** Typically 80% of gross invoice value disbursed upon invoice assignment.
2. **Factoring Reserve:** 20% retained by Factor until buyer pays in full.
3. **Deductions:**
   - *Factoring Service / Admin Fee:* Percentage of gross invoice (e.g., 1.0% to 2.0%).
   - *Discount / Financing Charge:* Interest charged on the advance amount for the credit period.
4. **Final Reserve Settlement:**
   $$\text{Final Balance Paid to Exporter} = \text{Reserve Amount} - \text{Service Fee} - \text{Discount Charge}$$

---

### Worked Problem 5: Factoring Cash Flow & Net Yield
**Question:**  
An engineering exporter assigns an export invoice of **USD 100,000** on 90-day D/A terms to an Export Factor under a non-recourse arrangement.  
Terms:
- Advance percentage: 80%
- Factoring service fee: 1.5% of total invoice value
- Financing / Discount charge: 8.0% p.a. on advanced funds
- Buyer pays the factor in full on day 90.

*Calculate: (a) Immediate cash advance disbursed, (b) Total factoring deductions, and (c) Final balance remitted to exporter on day 90.*

**Solution:**
1. **Immediate Cash Advance (80%):**
   $$\text{Immediate Advance} = 80\% \times \text{USD } 100,000 = \mathbf{USD\ 80,000}$$
   $$\text{Factoring Reserve (20%)} = \text{USD } 20,000$$
2. **Calculate Factor's Deductions:**
   - *Service Commission Fee (1.5% of Invoice):*
     $$\text{Service Fee} = 0.015 \times \text{USD } 100,000 = \text{USD } 1,500$$
   - *Financing / Discount Charge on Advance (8% p.a. for 90 days):*
     $$\text{Discount Charge} = \text{USD } 80,000 \times 0.08 \times \left(\frac{90}{365}\right) = \text{USD } 1,578.08$$
   - *Total Deductions:*
     $$\text{Total Deductions} = \text{USD } 1,500 + \text{USD } 1,578.08 = \mathbf{USD\ 3,078.08}$$
3. **Final Reserve Settlement (Day 90):**
   $$\text{Final Balance Paid} = \text{Reserve } (20,000) - \text{Total Deductions } (3,078.08) = \mathbf{USD\ 16,921.92}$$
4. **Total Net Realization by Exporter:**
   $$\text{Total Cash Realized} = \text{Initial Advance } (80,000) + \text{Final Settlement } (16,921.92) = \mathbf{USD\ 96,921.92}$$

---

## 6. Marine Insurance Claim & General Average Calculations

### A. Particular Average (Partial Loss) Settlement Formula
Under Section 71 of the Marine Insurance Act, 1963:

$$\mathbf{\text{Claim Payable} = \text{Depreciation Percentage} \times \text{Insured Sum}}$$

$$\text{Where: } \mathbf{\text{Depreciation Percentage} = \frac{\text{Gross Sound Market Value} - \text{Gross Damaged Market Value}}{\text{Gross Sound Market Value}}}$$

### B. General Average Contribution Formula
$$\mathbf{\text{General Average Contribution Rate } (C_r) = \frac{\text{Total General Average Loss / Expenditure}}{\text{Total Contributory Value of Adventure}}}$$

$$\mathbf{\text{Individual Party Contribution} = C_r \times \text{Contributory Value of that Party's Saved Property}}$$

---

### Worked Problem 6: Marine Claims & General Average
**Question:**  
(a) An export consignment of basmati rice insured for **USD 50,000** under ICC (A) suffers sea water damage during transit. Upon arrival at Dubai:
- Gross Sound Market Value (if undamaged) = USD 60,000
- Gross Damaged Market Value = USD 42,000  
*Calculate the marine insurance claim payable.*

(b) A cargo vessel grounds on a reef. To refloat the vessel, the captain orders 200 tons of cargo jettisoned (valued at **USD 100,000**) and incurs emergency tug assistance costs of **USD 50,000**. Total General Average loss = **USD 150,000**.  
The net values of saved property at the completion of the voyage are:
- Ship value = USD 1,500,000
- Total saved cargo value = USD 1,300,000
- Ocean freight at risk saved = USD 200,000  
*Calculate: (1) General Average contribution rate, and (2) The contribution payable by an exporter whose saved cargo is valued at USD 130,000.*

**Solution:**

**(a) Particular Average Claim:**
1. Calculate Depreciation Percentage:
   $$\text{Depreciation} = \frac{60,000 - 42,000}{60,000} = \frac{18,000}{60,000} = 30\%$$
2. Apply Depreciation to Insured Sum:
   $$\text{Claim Payable} = 30\% \times \text{USD } 50,000 = \mathbf{USD\ 15,000}$$

**(b) General Average Adjustment:**
1. Calculate Total Contributory Value of the Adventure:
   $$\text{Total Contributory Value} = \text{Ship } (1,500,000) + \text{Cargo } (1,300,000) + \text{Freight } (200,000) = \mathbf{USD\ 3,000,000}$$
2. Calculate Contribution Rate:
   $$\text{Contribution Rate } (C_r) = \frac{\text{Total GA Loss}}{\text{Total Contributory Value}} = \frac{150,000}{3,000,000} = 0.05 = \mathbf{5\%}$$
3. Calculate Exporter's Specific Contribution:
   $$\text{Exporter's Contribution} = 5\% \times \text{USD } 130,000 = \mathbf{USD\ 6,500}$$
   *(Note: This USD 6,500 contribution is fully reimbursed to the exporter by their marine cargo insurer under ICC A, B, or C).*
