# Messy-Medical-ETL
Extracted Transformed and Loaded
Right after learning about how statistics gets employed in Data Engineering, Here's my happy, satisfying practice session with a messy medical simulated messy dataset with Usability score of 5.88.
 - 100 rows and 10 columns
 - over 190 null values across 8 columns including Age and Gender
 - IMPORTANT Attributes (as we considered them) - ['Age', 'Gender', 'Blood_Pressure', 'BMI', 'Cholesterol', 'Smoker']
### Handling NULL values
 - Imputing with median
 - Imputing male and female randomly by maintaining the original proportion/probability of male to female
 - Dropped rows that had 2 or more missing values in the considered IMPORTANT Attributes
 - Hot (cold) Deck Imputation for Age -> Imputed Age with median values after clustering by Diagnosed disease
 - ML imputation using Multiple Imputation by Chained Equations (scikit-learn)
