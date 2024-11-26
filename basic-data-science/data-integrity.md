# Data Integrity

To ensure clean, accurate, and complete data to maintain integrity and avoid misleading insights.

---

## Importance of Data Integrity:

- **Risks to Integrity** : Errors during replication, transfer, manipulation, or human error can cause incomplete or inconsistent data.
- **Examples of Compromise**:
  - Incorrect date formats (e.g., DD/MM/YY vs. MM/DD/YY).
  - Incomplete replication or import issues during data transfer.
  - Erroneous removal of unique records during manipulation.
- **Solutions**:
  - Use standard formats and validate datasets thoroughly.
  - Follow company protocols for ensuring integrity.

## Common Data Constraints:

| **Data Constraint**      | **Definition**                                                           | **Example**                                                   |
| ------------------------ | ------------------------------------------------------------------------ | ------------------------------------------------------------- |
| **Type**                 | Must match predefined data types (e.g., date, number).                   | A date field cannot contain text.                             |
| **Range**                | Values must lie within acceptable limits.                                | A score must be between 0 and 100.                            |
| **Mandatory**            | Required fields cannot be empty.                                         | An "email" field cannot be left blank.                        |
| **Unique**               | No duplicate values allowed.                                             | Each user ID must be distinct.                                |
| **Regex Patterns**       | Must conform to specific formats (e.g., ###-###-#### for phone numbers). | A phone number must follow the pattern.                       |
| **Primary/Foreign Keys** | Ensure uniqueness and reference integrity in databases.                  | Primary keys cannot be duplicated.                            |
| **Set-Membership**       | Values must belong to a predefined set.                                  | Status field must be "Active" or "Inactive."                  |
| **Accuracy**             | Must reflect the real-world entity being measured.                       | Zip codes should match geographic areas.                      |
| **Completeness**         | All required data points must be present.                                | Profiles must include name and address.                       |
| **Consistency**          | Data must be identical across different collection points.               | A customer address should match in sales and billing systems. |

## Aligning Data with Business Objectives

Steps to Align Data with Business Objectives:

### 1. Identify Business Questions:

Define the question the data needs to answer (e.g., revenue generation, customer reviews).

### 2. Check for Data Cleanliness:

- Ensure data is free from duplicates, inaccuracies, or missing values.
- Example: Handle duplicate customer entries to avoid skewed calculations.

### 3. Evaluate Data Limitations:

- Assess if enough data is available or if alternate data sources are needed.
- Example: Incomplete sales data may require changes to the analysis process.

### 4. Data Processing Techniques:

- **VLOOKUP**: Quickly find and match data (e.g., activation dates or user details).

  `=VLOOKUP(lookup_value, table_array, col_index_num, [range_lookup])`

- **DATEDIF**: Calculate differences between dates (e.g., time from activation to first access).
  Clean data before performing analyses like attendance validation or session tracking.

## Key Takeaways:

- Clean Data + Alignment = Accurate Insights:
  - Clean the data to improve its usability.
  - Modify objectives or apply constraints when data partially aligns.
- Strategies for Better Alignment:
  - Validate data relevance and usability before analysis.
  - Address newly discovered variables with constraints or adjusted objectives.
