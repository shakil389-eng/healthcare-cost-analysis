# Healthcare Cost Analysis

US healthcare case study: how patient demographics (age, gender) and admission types relate to medical conditions, billing and hospital resource use. Built in Excel and presented as a PowerPoint deck. The findings feed two sets of recommendations: one for patients choosing an insurance provider, one for hospital planning.

## Project Files

| File | Description |
|------|-------------|
| `Healthcare analysis.xlsx` | Raw data, cleaned data, data dictionary, cleaning log, pivot tables and insight sheets |
| `healthcare analysis PPT.pptx` | Presentation summarising the findings and recommendations |

## Data

- **Records:** 10,000 patient admissions (Oct 2018 to Oct 2023), 9,976 with a usable billing amount
- **Key fields:** age, gender, blood type, medical condition, admission and discharge dates, insurance provider, billing amount (USD), admission type, test result
- **Conditions:** Arthritis, Asthma, Cancer, Diabetes, Hypertension, Obesity
- **Insurers:** Aetna, Blue Cross, Cigna, Medicare, UnitedHealthcare
- **Sample check:** every gender, age group, condition and insurer segment has an adequate sample size (95% margin of error of about 1-3%)

## Approach

1. Kept an untouched copy of the raw CSV and documented every column in a data dictionary
2. Cleaned data-quality issues (letter/digit mix-ups, inconsistent text, mixed date formats, blank billing amounts) and logged each fix
3. Removed patient name, doctor and hospital fields for privacy
4. Built pivot tables for condition, demographics, blood group, admission type and insurer
5. Tested hypotheses and turned the results into recommendations

## Key Findings

- **Medical condition is the biggest cost driver.** Cancer averages about $39.7K per admission, 3.2x Obesity (about $12.5K). Diabetes ($30.1K) is second highest. Overall average is $23.4K.
- **Age, gender and length of stay barely change billing.** Average billing is about $23.2K to $23.7K across age groups.
- **Admission type drives length of stay.** Emergency and urgent stays average about 15.5 days against about 10 for elective. Unplanned admissions are 69% of admissions but 78% of bed-days.
- **Emergency admissions bill about 4% above average** ($24.3K), while urgent admissions sit about 3% below ($22.7K).
- **Insurers differ by about 6% overall.** Cigna ($24.2K) and Aetna ($24.1K) are highest, Blue Cross ($22.8K) is lowest. Differences are larger by condition: Cancer ranges from $36.1K (Medicare) to $43.1K (Cigna), and Diabetes from $24.8K (UnitedHealthcare) to $32.2K (Blue Cross).
- **Demographic patterns:**
  - Hypertension is the largest group (2,155 cases, 21.6%), and 61% of those patients are male.
  - Asthma is most common in the young group.
  - Cancer and Arthritis rise with age.
  - Diabetes and Obesity are more common in women (58% and 62%).
- **Blood type has no strong link to condition.** Visits are spread evenly across blood groups.
- **Seasonality is mild.** Admissions peak in March (873) and are lowest in February (779). Hypertension peaks in October (214).

## Recommendations

**For patients choosing an insurer**
- Compare insurers for your specific condition, not just overall price. The gap between insurers is far larger for Cancer and Diabetes than overall.
- Blue Cross, Medicare and UnitedHealthcare average about 2-3% lower billing than the overall average.

**For hospital planning**
- Plan bed capacity around emergency and urgent admissions, which take most bed-days.
- Prepare for a high, steady volume of Hypertension cases all year.
- Focus cost management on Cancer and Diabetes, where billing per admission is highest.

## Tools Used

- Microsoft Excel (data cleaning, pivot tables, formulas, charts, power query editor)
- Microsoft PowerPoint

## Author

**Shakeel Nawaz Khan**
GitHub: [shakil389-eng](https://github.com/shakil389-eng)
