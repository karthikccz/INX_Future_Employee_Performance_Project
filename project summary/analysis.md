# Analysis

## Data preparation
The dataset contains 1,200 employees and 28 columns. There are no missing values and no duplicate rows. `EmpNumber` is excluded as an identifier. `PerformanceRating` is the target with levels 2, 3 and 4.

Categorical variables are one-hot encoded. Numerical variables are standardized for Logistic Regression. No PCA is used because the project requires interpretable business factors.

## Department performance

| Department | Employees | Average Rating | Rating 4 % | Rating 2 % |
|---|---:|---:|---:|---:|
| Development | 361 | 3.086 | 12.2% | 3.6% |
| Data Science | 20 | 3.050 | 10.0% | 5.0% |
| Human Resources | 54 | 2.926 | 11.1% | 18.5% |
| Research & Development | 343 | 2.921 | 12.0% | 19.8% |
| Sales | 373 | 2.861 | 9.4% | 23.3% |
| Finance | 49 | 2.776 | 8.2% | 30.6% |

## Top three factors

| Rank | Factor | Mean Permutation Importance |
|---|---|---:|
| 1 | EmpEnvironmentSatisfaction | 0.24 |
| 2 | EmpLastSalaryHikePercent | 0.23 |
| 3 | YearsSinceLastPromotion | 0.08 |

Spearman correlations with PerformanceRating were 0.40 for Employee Environment Satisfaction, 0.274 for Employee Last Salary Hike Percentage and -0.270 for Years Since Last Promotion.

The strongest department average is Development (3.086) and the lowest is Finance (2.776). Finance has 30.6% rating-2 employees in the supplied sample.

## Model results

Random Forest:
- Accuracy: 0.92
- Balanced accuracy: 0.83
- Weighted F1: 0.91
- Macro F1: 0.87

Logistic Regression baseline:
- Accuracy: 0.7583
- Balanced accuracy: 0.7576
- Weighted F1: 0.7730
- Macro F1: 0.6869

Permutation importance on the held-out test set is the main factor-selection technique because it measures how much predictive performance changes when an original feature is shuffled. These are predictive associations, not causal conclusions.
