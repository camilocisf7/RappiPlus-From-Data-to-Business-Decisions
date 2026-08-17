# RappiPlus-From-Data-to-Business-Decisions

## Contents

- [Business Objective](#Business-objective)

- [DataSet](#DataSet)

- [Data Preparation](#Data-Preparation)

- [Analysis](#Analysis)

- [Visualization](#Visualization)

- [Key Insights](#key-insights)

- [Recommendations](#recommendations)

**Business Objective:**

Evaluate RappiPlus’s commercial performance, customer journey, retention, and checkout experience to identify opportunities for improving conversion, profitability, and customer engagement.

**DataSet**

| Dataset | Contains | Purpose|
| -------- | -------- | -------- |
| Orders | Orders, products, prices, quantities, countries, devices | Revenue & profitability |
| Catalog| Product information and costs | Product analysis |
| Marketing | Channel-level marketing expenditure | Marketing analysis |
| User activity| User events and timestamps | Funnel & retention |
| Checkout experiment| Control/treatment and conversion | A/B testing |

**Data Preparation**

* Inspected missing values and duplicates.
* Standardized country and categorical values.
* Validated numerical fields such as quantity and price.
* Removed invalid order quantities according to project rules.
* Checked inconsistent event sequences.
* Validated relationships between orders and product information.

**Analysis**

* Calculated revenue, cost, profit and average ticket.
* Analyzed product sales and marketing expenditure.
* Built a user conversion funnel using SQL.
* Performed cohort retention analysis.
* Conducted a two-proportion z-test for the checkout experiment.

**Visualization**
* Built an executive dashboard in Tableau.
* Created KPI cards and business-focused visualizations.
* Highlighted conversion, profitability and customer behavior.
* 
**Key Insights:**

* 💰 9.49M revenue and 3.01M profit, with an estimated 31.8% profit margin.
* 📉 The checkout funnel revealed a potential event-tracking issue and a significant point of friction around payment information.
* 🧪 The new checkout UI increased observed conversion from 15.69% to 16.29%, but the difference was not statistically significant (p = 0.416).

**Recommendations**

1. Audit event tracking

Investigate why users can register add_to_cart without a corresponding select_item event before using the funnel for business decisions.

2. Investigate checkout friction

Analyze users who reach checkout but fail to provide payment information, segmenting by device, country and acquisition source.

3. Continue experimentation

The observed improvement in conversion was not statistically significant. Before implementing the new UI globally, run a larger or longer experiment and analyze results by customer segment.
