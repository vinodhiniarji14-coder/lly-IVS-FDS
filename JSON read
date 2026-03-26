# Importing necessary libraries
import pandas as pd
from pandas import json_normalize
# Sample nested JSON data
data = {
 "students": [
 {"name": "Ram", "details": {"age": 20, "marks": 85}},
 {"name": "Sita", "details": {"age": 19, "marks": 90}},
 {"name": "Ravi", "details": {"age": 21, "marks": 78}}
 ]
}
# Convert JSON data into DataFrame
df = json_normalize(data["students"])
# Display the flattened DataFrame
print("Flattened DataFrame from JSON:")
print(df)
