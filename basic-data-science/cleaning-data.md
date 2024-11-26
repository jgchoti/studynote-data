# What is Dirty Data?

Dirty data refers to information that is incomplete, incorrect, or irrelevant, making it unreliable for analysis. It can take various forms:

## Types of Dirty Data:

| **Type of Dirty Data**        | **Description**                            | **Causes**                                    | **Impact**                                 |
| ----------------------------- | ------------------------------------------ | --------------------------------------------- | ------------------------------------------ |
| **Duplicate Data**            | Records appearing more than once           | Manual entry errors, batch imports, migration | Skewed metrics, inflated counts, confusion |
| **Outdated Data**             | Old data needing replacement               | Changes in roles or obsolete systems          | Poor insights, flawed decision-making      |
| **Incomplete Data**           | Missing critical fields                    | Collection or entry errors                    | Reduced productivity, disrupted services   |
| **Incorrect/Inaccurate Data** | Complete but incorrect data                | Human error, fake/test data                   | Misleading insights, revenue loss          |
| **Inconsistent Data**         | Variations in formatting or representation | Improper storage, transfer errors             | Confusion, classification challenges       |

---

## Causes of Dirty Data:

- Human errors in entry and processing.
- Data transfer issues, such as duplication or formatting inconsistencies.
- Use of outdated or incorrect collection methods.

## Data Quality Dimensions:

| **Dimension**    | **Definition**                                                  | **Example**                                                                     |
| ---------------- | --------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| **Validity**     | Ensuring data conforms to defined business rules or constraints | Data from five years ago uses outdated technology not supported by the business |
| **Accuracy**     | Degree of conformity of a measure to a standard or true value   | Business database addresses differ from public postal service database          |
| **Completeness** | Degree to which all required measures are known                 | NULL or missing value for "Number of employees per store"                       |
| **Consistency**  | Degree to which a set of measures is equivalent across systems  | Store opening dates stored in both MM/DD/YYYY and MM/YY formats                 |

## Common Mistakes to Avoid in Data Cleaning

| **Mistake**                                       | **Description**                                                                                                  | **Example**                                                                                                      |
| ------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| **Not checking for spelling errors**              | Misspelled words may go unnoticed, especially names or addresses.                                                | “John” entered as “Jon” in some instances in customer data.                                                      |
| **Forgetting to document errors**                 | Failing to document fixes can lead to repeating the same errors without a quick reference.                       | Not noting the error in date formatting when troubleshooting a formula.                                          |
| **Not checking for misfielded values**            | Values entered in the wrong fields may not be easily noticed but can cause errors later.                         | “Spain” entered in the city column instead of the country column.                                                |
| **Overlooking missing values**                    | Missing data can distort calculations and analysis, leading to inaccurate conclusions.                           | Missing week of transactions while calculating total sales.                                                      |
| **Only looking at a subset of the data**          | Focusing on a partial dataset can lead to missing errors or incomplete analysis.                                 | Cleaning only one data source in a bird migration dataset, missing duplicated data from another source.          |
| **Losing track of business objectives**           | Getting distracted by interesting patterns or data points not related to the task can cause loss of focus.       | Discovering snowfall patterns while analyzing rainy days but losing focus on the primary task.                   |
| **Not fixing the source of the error**            | Addressing the symptoms of errors without fixing the root cause can result in recurring issues.                  | Continuously fixing spreadsheet errors without setting up standardized data entry rules.                         |
| **Not analyzing the system prior to cleaning**    | Failing to understand where dirty data originates from can lead to repeated mistakes during cleaning.            | Not investigating whether errors are due to data entry or system issues before starting the cleaning process.    |
| **Not backing up data prior to cleaning**         | Not creating a backup can result in data loss or errors after changes.                                           | Not backing up data before cleaning, losing valuable information when the program crashes.                       |
| **Not accounting for data cleaning in deadlines** | Underestimating the time required for data cleaning can impact project deadlines and result in missed timelines. | Not accounting for data cleaning time in the project schedule, causing delays in delivering analysis or reports. |

## Challenges in Merging Datasets

- Inconsistent Formats: Different datasets may have different formats for similar data points. For example:
  - Address information might be split into multiple columns in one dataset (e.g., suite, apartment number) and combined into one column in another.
  - Member IDs could be represented as numbers in one dataset and email addresses in another.
  - Membership types might differ in terminology (e.g., “Young Professional” vs. “Student Associate”), which requires standardizing the terminology.
- Duplicates: Different datasets might have the same person listed in multiple ways (e.g., different member IDs, names, etc.), so removing duplicates is crucial.
- Data Compatibility: Ensuring the datasets can work together requires checking for consistency, matching schemas, and understanding the structure of each dataset.

## Key Questions Before Merging Datasets

### Do I have all the data I need?

- Ensure you have all relevant information, such as customer details, transactions, and other necessary data for your analysis.

### Does the data I need exist within these datasets?

- Evaluate if the datasets contain all the data required for your analysis.
- Look for relevant fields and confirm if they are present.

### Do the datasets need cleaning or are they ready for use?

- Check the quality of data in both datasets.
- Determine if there are missing values, duplicates, or inconsistencies that need to be addressed before merging.

### Are the datasets cleaned to the same standard?

- Ensure that both datasets are cleaned to the same standards (e.g., handling missing values, data formatting, updating timestamps, etc.).

### Tools for Data Merging and Cleaning

- Spreadsheet Tools: You can clean, merge, and prepare datasets for analysis directly within spreadsheet software like Excel or Google Sheets.
- SQL Queries: SQL can be used for more complex data cleaning and merging tasks, especially when working with large databases.
- Programming Languages (e.g., R): For advanced data manipulation, languages like R are highly useful. They allow for extensive data cleaning, merging, and analysis capabilities.

## Key Takeaways:

- Clean data ensures effective, accurate analysis and decision-making.
- Regularly cleaning and auditing datasets to eliminate errors and inconsistencies is crucial to avoid costly mistakes.
- By adopting proper processes and tools, you can significantly mitigate the risks associated with dirty data.
- Data merging involves combining data from different sources, which often requires handling inconsistencies and resolving duplicate entries.
- Asking the right questions beforehand helps ensure that the datasets are compatible and clean.
- The choice of tools depends on the complexity of the task, the volume of data, and your technical expertise.
