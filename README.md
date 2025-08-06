# \# Salifort Motors: Employee Turnover Prediction

# 

# \## Project Overview

# This project analyses HR data from Salifort Motors to predict employee turnover and provide actionable recommendations to improve retention.  

# Models were built using Logistic Regression, Decision Tree, and Random Forest, the latter achieving the best performance.

# 

# ---

# 

# \## Dataset

# \- \*\*Rows:\*\* 15,000 employees (after cleaning: 11,991)

# \- \*\*Columns:\*\* Satisfaction level, performance evaluation, projects, average monthly hours, tenure, work accidents, promotions, department, salary, and turnover flag.

# \- \*\*Target Variable:\*\* `left` (1 = employee left, 0 = stayed)

# 

# ---

# 

# \## Key Insights

# \- 50% of employees work overtime (>200 hrs/month) → strong driver of turnover.

# \- Low promotion rates (1.7%) which reduces retention.

# \- Low \& medium salary employees more likely to leave.

# \- Employees with extreme workloads (too many or too few projects) tend to resign.

# 

# ---

# 

# \## Modeling

# | Model                | Accuracy | Recall | Precision | AUC   |

# |----------------------|----------|---------|-----------|-------|

# | Logistic Regression  | 82%      | 27%     | 44%       | 0.60  |

# | Decision Tree        | 97.8%    | 91.5%   | 95.2%     | 0.975 |

# | \*\*Random Forest\*\*    | \*\*98.3%\*\*| \*\*93.4%\*\*| \*\*96.7%\*\*| \*\*0.963\*\* |

# 

# Random Forest was selected as the champion model.

# 

# ---

# 

# \## Recommendations

# \- Reduce overtime by hiring additional staff.

# \- Provide promotions and recognition to high performers.

# \- Balance project allocation (ideal: ~3 projects per employee).

# \- Retention strategies for employees in first 3 years of tenure.

# 

# ---

# 

