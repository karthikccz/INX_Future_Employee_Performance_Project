# Summary and Recommendations

## Business answers

**Department performance:** Performance differs across departments. Development has the highest average rating in the supplied sample, while Finance has the lowest and the highest proportion of rating-2 employees.

**Top three factors:** Employee Environment Satisfaction, Employee Last Salary Hike Percentage, and Years Since Last Promotion.

**Prediction model:** The Random Forest achieved 93.33% accuracy, 85.33% balanced accuracy and 93.13% weighted F1 on the held-out test set.

## Recommendations

1. Review departments with higher proportions of lower performance ratings and identify department-specific operational causes.
2. Strengthen employee-environment practices through structured feedback, manager support, role clarity and workload reviews.
3. Review salary-hike practices and communicate reward criteria clearly.
4. Identify employees with longer promotion gaps and provide transparent career-development and progression plans.
5. Use the prediction model as decision support, not as the sole basis for hiring, promotion or penalties.
6. Revalidate the model periodically as new employee-performance data becomes available.

## Limitations

The data is observational and represents a supplied snapshot. It does not prove causation. The target is imbalanced, model performance depends on the train/test split, and feature importance may change with new samples or model configurations. Any real employment use should include human review and job-related validation.
