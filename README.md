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

---

## ✴️ Methods of Hypothesis Test conclusions
Compare a calculated test statistic to a critical value
- If test statistic > Critical value, reject H₀
- If test statistic < Critical value, fail to reject H₀

*Compare p-value to the alpha risk*

- If p-value < alpha risk, reject H₀
- If p-value > alpha risk, fail to reject H₀

---

## ☢️ Statistical & Practical Significance of Hypothesis test
### ‼️Significant but not Practical:
Assume that a Steel manufacturing company is comparing two methods of fulfilling customer orders in which the new method is significantly faster than the standard ones by 1 hour, however to justify the cost of changing to the new method, a reduction of 2 hours is required

### ⁉️Practical but not Significant:
Assume that a bank call center is piloting new technology to process payments which has increased transactions by 500 per day. Although the new technology has a higher average that will have a practical impact to the business there is no statistically significant difference since p ≥ 0.05

---

## 🛃 Case Study: Hypothesis testing by the Quality Manager in a Steel manufacturing plant
### 🈲 Objectives

1. Sample size estimation for defect detection
2. Cycle time comparison before and after improvement for Casting & Rolling machines
3. One tailed Z-test for Thickness validation for Casting & rolling machines
4. Comparing planning performance based on shifts using T-Test

---

### ☯️ Interpretation

1. *Situation 1: The Quality Manager looks at the Planning Resource data that is continuous. Currently, the population Standard Deviation for Casting & Rolling are at 19 units and 49 units respectively. Now, the Manager wants to decide the size of a sample that can improve the defect rate within ±10 units tolerance with 90% confidence level*

      **Inference**: From the excel calulation, it is recommended to have the sample size:  
                     - for casting, with a range between 70 to 90 data points
                     - for rolling, with a range between 60 to 80 data points

   *Situation 2: Later the Quality Manager realized that one of the machine outputs is defective. The non-defective population proportion for casting machine is 70%. Now, the Manager wants to decide the sample size to draw the sample that can estimate the proportion of compliant steel sheets within ±20 units tolerance with 90% confidence level*

      **Inference**: From the excel calculation, for casting, it is recommended to have a sample size ranging between 50-80 data points

3. *Situation: After the joint regional meeting, the company decided to upgrade casting and rolling machines in the plant that can improve the cycle time for better efficiency and faster customer delivery. As a part of testing, sample size of 100 data points are considered to compare the performance of old and new machines for casting and rolling operations respectively. The significance level is 0.05 but the manager is unsure of the confidence interval which is to be calculated manually*
   
      **Inference**: T.Test performance value for both casting and rolling machines is 0.5392. It means that 53.92% probability that the difference observed between the two                      samples is due to random chance. Since 0.5392 > 0.05, it is not statistically significant.
   
      **Conclusion**: 1. Fail to reject the null hypothesis (H₀)
                      2. There is no evidence of a statisitcally significant difference between the two sample groups. Hence, we cannot confidently claim that the groups                             are different based on this data

4. *Situation: Now, the Quality Manager, wants to validate the thickness for both casting & rolling machines. Because the new machinery supplier claims that the steel sheets are thinner when compared to the older machines. 
*"In God we trust. All other must bring data" - W. Edwards Deming*
