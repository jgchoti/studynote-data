# Statistical Power and Proxy Data

## Statistical Power

**Definition**: Statistical power is the probability of detecting a true effect in a test or study. It is represented as a value between 0 and 1 (e.g., 0.8 = 80% power).
**Importance**: Ensures meaningful results by minimizing the likelihood that findings are due to random chance.
**Minimum Threshold**: A statistical power of at least 0.8 (80%) is typically required to consider results reliable and statistically significant.
**Influencing Factors**:

- **Sample size**: Larger sample sizes increase power by reducing random variability.
- **Study design**: Must control for external factors that could influence results (e.g., promotions, location-specific differences).
- **Hypothesis testing**: Focus on measurable effects like increased sales or customer count.

## Proxy Data

**Definition**: Proxy data is alternative data used when direct data is unavailable. It provides estimates or predictions to support business objectives.

**Examples**:

- **Car Dealership**: Use website clicks on car specs as a proxy for potential sales.
- **Plant-Based Product**: Use sales data of similar products as a proxy for demand forecasts.
- **Tourism Campaign**: Use historical booking data after previous campaigns to predict outcomes.
- **Vaccine Contraindications**: Use open dataset trial results as a proxy for potential contraindications.

## Open or Public Datasets

**Definition**: Freely available datasets from repositories like Kaggle, often used when internal data is insufficient.

### Dataset Formats:

- CSV: Easy-to-read data (e.g., credit card customer profiles).
- JSON: Structured data for complex applications (e.g., YouTube trending videos).
- SQLite: Relational database for historical trends (e.g., wildfire data).
- BigQuery: Scalable datasets for advanced analytics (e.g., Google Analytics samples).

### Best Practices:

- Check for duplicates and null values.
- Understand how null values are treated (e.g., unassigned vs. "0").
- Ensure proxy data matches the population or use case it represents.

## Key Takeaways

- Statistical Power: Achieve at least 80% power by optimizing sample size and controlling external factors.
- Proxy Data: A useful alternative when direct data isn't available, but it must closely align with the intended analysis.
- Data Preparation: Always pre-clean datasets by identifying duplicates, null values, and ensuring data suitability.
