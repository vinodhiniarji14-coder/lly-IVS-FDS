# Importing required libraries
import requests
from bs4 import BeautifulSoup
import pandas as pd
# Sample HTML content (can also use a webpage URL)
html_data = """
<table>
<tr><th>Name</th><th>Age</th><th>Marks</th></tr>
<tr><td>Ram</td><td>20</td><td>85</td></tr>
<tr><td>Sita</td><td>19</td><td>90</td></tr>
<tr><td>Ravi</td><td>21</td><td>78</td></tr>
</table>
"""
# Parse the HTML data using BeautifulSoup
soup = BeautifulSoup(html_data, 'html.parser')
# Extract table rows
rows = []
for tr in soup.find_all('tr'):
 cols = [td.text for td in tr.find_all(['td', 'th'])]
 rows.append(cols)
# Convert to DataFrame
df = pd.DataFrame(rows[1:], columns=rows[0])
# Display the DataFrame
print("Extracted DataFrame from HTML Table:")
print(df)
