<!-- ELUCENIA technical documentation · nrs-2002 · en · no clinical/professional/rights approval -->

# NRS-2002

[conditions, sources and permissions](https://elucenia.org/en/tools/nrs-2002)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### Impaired nutritional status

`estado`

- `0` — Absent: normal nutritional status
- `1` — Mild: weight loss \> 5% in 3 months or intake of 50% to 75% of requirements in the last week
- `2` — Moderate: loss \> 5% in 2 months, or BMI 18.5 to 20.5 with impaired general condition, or intake of 25% to 60%
- `3` — Severe: loss \> 5% in 1 month (\> 15% in 3 months), or BMI \< 18.5 with impaired general condition, or intake of 0% to 25%

### Disease severity (increased requirements)

`gravidade`

- `0` — Absent: normal nutritional requirements
- `1` — Mild: hip fracture, chronic disease with an acute complication (cirrhosis, COPD, hemodialysis, diabetes, cancer)
- `2` — Moderate: major abdominal surgery, stroke, severe pneumonia, hematologic malignancy
- `3` — Severe: head injury, bone marrow transplant, ICU with APACHE II \> 10

### Age ≥ 70 years

`idade`

## Method edition

NRS 2002/ESPEN Kondrup 2003: 2 domains 0–3, age≥70 +1, total 0–7

## Documented formula

Score = impaired nutritional status (0 to 3) + disease severity (0 to 3) + 1 point if age ≥ 70 years. Total 0 to 7.

Score ≥ 3: nutritional risk.

## Limits and population

NRS-2002 is risk screening based on the combination of nutritional status and disease severity. Its development distinguished study groups more likely to benefit; a total does not guarantee an individual response or prescribe the route or dose of nutritional support. Definitions, eligibility and age must match the version.

## References

- [Kondrup J et al. Nutritional risk screening (NRS 2002): a new method based on an analysis of controlled clinical trials. Clin Nutr, 2003.](https://doi.org/10.1016/S0261-5614(02)00214-5)

- [Kondrup J et al. ESPEN guidelines for nutrition screening 2002. Clin Nutr, 2003.](https://doi.org/10.1016/S0261-5614(03)00098-0)

## Reproduce the technical tests

Run node test.cjs in the root directory of this repository to repeat the recorded synthetic cases. Original inputs, expectations and tolerances are preserved. Technical tests do not constitute clinical validation.

```sh
node test.cjs
```

tool.json contains sources, edition and review scope. examples.json retains synthetic inputs and expectations; results.json records the obtained results.

[Record and references](../tool.json) · [JavaScript code](../calculator.js) · [Reference cases](../examples.json) · [results.json](../results.json)

## Review and conditions of use

Independent clinical review has not been performed.

This interface is an authorial translation, not an official or certified edition. Independent clinical review, professional language review and instrument rights clearance have not been performed.

Formula or classification result. Interpretation, care and applicability depend on professional assessment and the selected source.

## License and attribution

Apache-2.0 applies only to ELUCENIA code. Rights to instruments, publications, translations and data remain with their respective holders. Preserve LICENSE and NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
