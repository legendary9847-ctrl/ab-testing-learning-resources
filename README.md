# A/B Testing: A Practical Beginner's Guide

## Introduction to A/B Testing

A/B testing (also called split testing) compares two versions of a webpage, advertisement, email, or product feature to learn which performs better against a defined goal.

- **Control (Version A):** The existing experience.
- **Variation (Version B):** The alternative experience being tested.
- **Goal:** A measurable action, such as a purchase, registration, or click.

### Basic workflow

1. Define one clear goal and a hypothesis.
2. Choose the element to test, such as a headline or call-to-action button.
3. Randomly assign eligible users to Version A or Version B.
4. Keep other important conditions as consistent as possible.
5. Collect enough data and compare the results.
6. Decide based on the results, uncertainty, and practical impact.

**Example hypothesis:** “Changing the button text from ‘Register’ to ‘Create my account’ will increase completed registrations.”

## Conversion Rate Calculation

The conversion rate is the percentage of visitors who complete the chosen goal.

**Formula:**

`Conversion rate = (Number of conversions / Number of visitors) × 100`

### Example

| Metric | Version A | Version B |
|---|---:|---:|
| Visitors | 1,000 | 1,000 |
| Purchases | 50 | 70 |
| Conversion rate | 5% | 7% |

Version A: `(50 / 1,000) × 100 = 5%`

Version B: `(70 / 1,000) × 100 = 7%`

Version B is higher by **2 percentage points**. That is a **40% relative increase** compared with Version A: `((7% - 5%) / 5%) × 100`.

A higher observed rate does not, by itself, prove that Version B is truly better. Random variation can produce differences in a sample.

## Statistical Significance

Statistical testing helps assess whether the observed difference would be unusual if there were no real difference between the versions, under the test's assumptions.

- **Null hypothesis (H₀):** The versions have equal underlying conversion rates.
- **Alternative hypothesis (H₁):** The underlying conversion rates differ.
- **P-value:** The probability, assuming the null hypothesis and model are correct, of observing results at least as extreme as those obtained.
- **Significance level:** A threshold chosen before analysing results, often 0.05.

If the p-value is below 0.05, the result is conventionally called statistically significant at the 5% level. If it is 0.05 or higher, the result is not statistically significant at that level. Neither outcome proves that a hypothesis is certainly true or false.

Sample size matters: small samples often give imprecise estimates and may not detect a meaningful effect. Plan the sample size in advance based on the baseline conversion rate, the smallest worthwhile effect, significance level, and desired statistical power. Also consider the size and business value of the improvement—not just statistical significance.

## Common Testing Mistakes

1. **Stopping too early:** Do not end a test just because one version is temporarily ahead.
2. **Using too little data:** Small samples can make conversion rates unstable.
3. **Changing several things at once:** This makes it harder to identify which change affected the result.
4. **Unequal or biased groups:** Use random assignment and check that tracking works consistently.
5. **Ignoring context:** Traffic sources, weekdays, promotions, and seasonal effects can influence outcomes.
6. **Choosing the winner by conversion rate alone:** Check statistical evidence and practical impact.
7. **Misreading the p-value:** It is not the probability that the result is wrong or that the null hypothesis is true.
8. **Forgetting the original goal:** Analyse the primary metric defined before the test and be mindful of other important outcomes.

## Useful Online Resources

- [A/B Test Statistical Significance Calculator](https://freestatisticaltools.com/ab-test-significance-calculator/?utm_source=chatgpt.com) — enter visitor and conversion counts for two versions to help examine the statistical evidence.
- [Optimizely: A/B Testing](https://www.optimizely.com/optimization-glossary/ab-testing/) — an overview of A/B testing concepts and use cases.
- [Google Analytics](https://analytics.google.com/) — a platform for measuring website and user behaviour; configure events and conversions to match your experiment goals.

**Reminder:** A calculator supports analysis, but it does not replace sound experimental design. Confirm that the calculator's statistical method fits your data, and interpret its output alongside sample size, effect size, and business context.

---

*This guide is for educational purposes. Choose your metrics and analysis plan before starting an experiment, and document any assumptions or limitations.*
