# AB_Testing_Projects
## Mobile App Subscription Screen A/B Test

## Technologies Used

- Python
- Pandas
- NumPy
- SciPy
- Matplotlib
- Jupyter Notebook

## Project Overview
This project analyzes an A/B test conducted in a mobile application to evaluate whether an alternative subscription screen design can improve conversion rates.
After onboarding, users are offered a weekly subscription priced at $4.99. The existing screen presents the subscription at its regular price, while the experimental version highlights the same price as a "50% discount" offer.
The goal of the experiment was to determine whether the new design increases the percentage of users purchasing the subscription.

## Business Problem
The current subscription screen converts approximately 17% of users who reach the paywall.
The product team proposed a new design emphasizing a 50% discount message while keeping the subscription price unchanged.
The business objective was to verify whether the alternative design could significantly increase subscription purchases and overall revenue per user.

## Experiment Design

### Population

Users who:

- Installed the mobile application
- Completed onboarding
- Reached the subscription screen

### Traffic Allocation

Users were randomly assigned into two groups:

- Control Group (A): Existing subscription screen
- Treatment Group (B): Alternative design with a "50% discount" message

User assignment remained fixed throughout the experiment.

### Primary Metric

Conversion Rate

Conversion Rate =

(Number of subscription purchases) /
(Number of users who viewed the subscription screen)

### Secondary Metric

Net Revenue Per User

Net Revenue Per User =

(Total subscription revenue) /
(Number of users who viewed the subscription screen)

## Hypotheses

### Null Hypothesis (H₀)

The alternative subscription screen does not increase conversion rate.

### Alternative Hypothesis (H₁)

The alternative subscription screen increases conversion rate.

## Statistical Method

To evaluate statistical significance, a two-proportion hypothesis test was performed.

Significance level:

- α = 0.05

The analysis was conducted in Python using SciPy.

## Results

| Metric | Control (A) | Variant (B) |
|----------|----------|----------|
| Conversion Rate | 6.1% | 8.9% |
| Revenue per User | $0.30 | $0.44 |

### Conversion Lift

Absolute Lift:

8.9% − 6.1% = 2.8 percentage points

Relative Lift:

(8.9% − 6.1%) / 6.1% = 45.9%

### Revenue Lift

$0.44 − $0.30 = $0.14 per user
## Conclusion

The A/B test demonstrated a statistically significant increase in conversion rate for the alternative subscription screen.

Key findings:

- Conversion rate increased by 45.9%
- Revenue per user increased by $0.14
- The observed effect remained stable throughout the experiment

Recommendation:

Deploy the new subscription screen to all users and continue monitoring key metrics for an additional two weeks after release.
