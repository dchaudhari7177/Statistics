
### Explanation of the Cleaning Steps:
1. **Filling Missing Values:**
   - **Age:** Missing age values are replaced with the median value of the age column. Median is chosen because it is less sensitive to outliers than the mean.
   - **Cabin:** Missing cabin values are filled with the string 'Unknown'. In some cases, you may choose to drop this column, but filling with 'Unknown' helps preserve the feature.
   - **Embarked:** Missing embarkation port values are filled with the most frequent value (mode). This is because embarkation ports have limited unique values.
   - **Fare:** Missing fare values are replaced with the median fare.
   - **SibSp and Parch:** Missing family-related values are assumed to be 0 (indicating no siblings/spouses or parents/children aboard).
   
2. **Handling Inconsistencies:**
   - The **Sex** column values are converted to lowercase to ensure consistency and avoid case-sensitivity issues.

3. **Handling Duplicates:** 
   - Duplicate rows (if any) are removed to ensure each passenger is unique.

4. **Data Type Conversion:**
   - Ensuring columns like `Survived` are of appropriate data types (e.g., integers for categorical values).

5. **Saving the Cleaned Dataset:**
   - The cleaned dataset is saved to a new CSV file called `Cleaned_Titanic_Dataset.csv`.

### Outcome:
- After cleaning, the dataset will have no missing values, all data will be formatted consistently, and the data types will be appropriate for analysis.
