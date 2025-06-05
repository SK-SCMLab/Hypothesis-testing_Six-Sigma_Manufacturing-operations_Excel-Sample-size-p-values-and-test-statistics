# 🈸 Hypothesis-testing_Six-Sigma_Manufacturing-operations_Excel (Significance of test)
This repository demonstrates how to conduct statistical hypothesis testing using Excel, including: 
- Sample size estimation
- Calculation of p-values
- Test statistics (z-test & t-test)
- One-tailed and two-tailed probabilities

---

## 🉑 Sample size estimation
Sample size can be calculated by answering three simple questions
-> How much variation present in the population? (σ)
-> At what interval or tolerance does the true population mean need to be estimated? (±Δ)
-> How much representation error is allowed in the sample? (α)

The sample size (n) of continuous data can be determined by the formula: 
**n = [(Z₁₋α/₂*σ)/Δ]^2**

The sample size (n) for discrete data can be determined by the formula:
**n= [(Z₁₋α/₂)/Δ]^2*p(1-p)**; σ = sqrt(p(1-p)
'p' is the % of non-defective

---

## 🈺 P-value
The p-value is the probability that any differences observed are due to random chance or common cause variation
- A small p-value indicates a small probability that the observed results could happen under the assumption that the null hypothesis is true
- Low p-values lead us to reject the null hypothesis
- If lower than alpha risk, the null is rejected in favor of the alternative
- High p-values indicate that we haven't gathered sufficient data or evidence to not reject the null hypothesis

---

## 🈷️ Test statistics
- The test statistics is calculated based on the observations
- A test statistic is used to determine the validity of a hypothesis test
- If the null hypothesis is true, the test statistic will be random variable with known distribution
- If we can conclude that the test statistic came from the population, then the null is not rejected
- The calculation of test statistic and critical value will depend on the particular hypothesis test
- If it is not likely for the test statistic to come from population, then the null is rejected

---

## 🆚 2-tailed and 1-tailed probability
- Use of 2-tailed probability and 1-tailed probability depends on the direction of the alternative hypothesis
- If the alternative hypothesis tests more than one direction, either less or more, use a 2-tailed probability value from the test, i.e., Mean (A) ≠ Mean (B)
- If the alternative hypothesis tests are one direction, use a 1-tailed probability value from the test, i.e., Mean (A) > Mean (B)

