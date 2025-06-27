# Credit Scoring Business Understanding

The Influence of the Basel II Accord on Model Selection
The Basel II Accord, and subsequent Basel III framework, mandates that financial institutions hold adequate capital reserves against various risks, with credit risk being a primary focus. The accord allows banks to use their own internal models to calculate these capital requirements, but only if these models are approved by regulators. This regulatory oversight creates a strong need for credit risk models that are not only accurate but also interpretable and well-documented.

An interpretable model, such as one built with logistic regression and Weight of Evidence (WoE), allows the bank to clearly explain to regulators how the model arrives at its conclusions. The decision-making process of the model is transparent, and the influence of each variable on the final credit score can be easily understood. This transparency is crucial for demonstrating to regulators that the bank has a sound and prudent approach to risk management. A well-documented model provides a clear audit trail of the model's development, validation, and implementation, further satisfying regulatory requirements.

The Necessity and Risks of a Proxy for "Default"
In many real-world credit scoring scenarios, a direct and clean "default" label is not readily available. Data may not be perfectly labeled, or the definition of default may be ambiguous. In such cases, it is necessary to create a proxy variable for default. This proxy is an engineered variable that uses available data to approximate the event of a borrower defaulting on their loan. For example, a proxy could be defined as a borrower being more than 90 days past due on a payment.

Trade-offs Between Simple and Complex Models in a Regulated Context
In the context of credit scoring within a regulated financial institution, there is a fundamental trade-off between the predictive power of a model and its interpretability.

Simple, Interpretable Models (e.g., Logistic Regression with WoE): These models are transparent and easy to explain. The impact of each variable on the final score is clear, which is a significant advantage in a regulated environment where model explainability is paramount. Regulators, auditors, and business stakeholders can readily understand how the model works. However, these models may not capture complex, non-linear relationships in the data, and their predictive accuracy might be lower than that of more complex models.

Complex, High-Performance Models (e.g., Gradient Boosting): These models, often referred to as "black-box" models, can capture intricate patterns in the data and generally offer higher predictive accuracy. This can lead to better risk differentiation and potentially higher profits. However, their lack of interpretability is a major drawback in a regulated industry. It is difficult to explain why the model made a particular decision.