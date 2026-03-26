# Importing necessary libraries
import pandas as pd
import numpy as np
# Creating a sample dataset with missing and outlier values
data = {
 'Marks': [85, 90, np.nan, 95, 100, 30, 110, np.nan, 88, 92]
}
df = pd.DataFrame(data)
print("Original Dataset:")
print(df)
# Handling Missing Values - Imputation with Mean
mean_value = df['Marks'].mean()
df['Marks'].fillna(mean_value, inplace=True)
print("\nAfter Handling Missing Values (Imputed with Mean):")
print(df)
# Handling Outliers - Filtering
# Assuming valid marks are between 0 and 100
filtered_df = df[(df['Marks'] >= 0) & (df['Marks'] <= 100)]
print("\nAfter Removing Outliers:")
print(filtered_df)
