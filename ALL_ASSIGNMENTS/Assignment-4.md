
## 1. Write a Python script to simulate the Central Limit Theorem using the Score column from the score.csv dataset. Draw 1000 samples of size 50, calculate the mean of each sample, and plot the distribution of these sample means. Also, calculate and print the mean of the sampling distribution and compare it with the actual mean of the Score column.




```python

# Importing necessary libraries
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
from google.colab import files
import io

# Step 1: Upload the CSV file
uploaded = files.upload()

# Step 2: Read the CSV file
# Assuming the user uploaded only one file, we get its key and read the CSV
file_name = next(iter(uploaded))
df = pd.read_csv(io.BytesIO(uploaded[file_name]))

# Step 3: Check the contents of the CSV file (optional)
print(df.head())

# Step 4: Extract the Score column (ensure the column name is correct)
if 'Score' in df.columns:
    scores = df['Score']
else:
    raise ValueError("The CSV file does not contain a 'Score' column.")

# Step 5: Initialize variables for Central Limit Theorem simulation
num_samples = 1000
sample_size = 50
sample_means = []

# Step 6: Generate 1000 samples and calculate the mean of each sample
for _ in range(num_samples):
    sample = np.random.choice(scores, sample_size)
    sample_means.append(np.mean(sample))

# Step 7: Plot the distribution of sample means
plt.figure(figsize=(10, 6))
sns.histplot(sample_means, kde=True, color='blue', bins=30)
plt.title('Distribution of Sample Means (Central Limit Theorem)')
plt.xlabel('Sample Mean')
plt.ylabel('Frequency')
plt.grid(True)
plt.show()

# Step 8: Calculate and print the mean of the sampling distribution
sampling_mean = np.mean(sample_means)
print(f"Mean of the sampling distribution: {sampling_mean}")

# Step 9: Calculate and print the actual mean of the Score column
actual_mean = np.mean(scores)
print(f"Actual mean of the Score column: {actual_mean}")

# Step 10: Compare the two means
print(f"Difference between sampling mean and actual mean: {abs(sampling_mean - actual_mean)}")


```

## The below is the colab link of the solution
[colab](https://colab.research.google.com/drive/1q1-dFnT-Fox0Y0-DWDMc7-9zSJAPwCVV)










# Approach for Central Limit Theorem Simulation

1. **Import Libraries**:  
   The necessary libraries are imported at the beginning, including `numpy`, `pandas`, `matplotlib.pyplot`, and `seaborn`. Additionally, the `files` and `io` modules are imported to handle file uploads in Google Colab.

2. **Upload CSV File**:  
   The user uploads a CSV file using `files.upload()`, which opens a file dialog to select and upload the CSV. The `next(iter(uploaded))` retrieves the file name for further operations.

3. **Read CSV File**:  
   The uploaded CSV file is read into a pandas DataFrame (`df`) using `pd.read_csv(io.BytesIO(uploaded[file_name]))`. The `io.BytesIO` ensures the file is read correctly in binary mode.

4. **Check Contents**:  
   The contents of the DataFrame are optionally displayed using `df.head()` to preview the first few rows of the data.

5. **Extract 'Score' Column**:  
   The 'Score' column is extracted from the DataFrame into a variable `scores`. An error is raised if the column doesn't exist.

6. **Set Variables for Simulation**:  
   Variables are initialized for the Central Limit Theorem simulation:  
   - `num_samples` is set to 1000 for the number of samples.
   - `sample_size` is set to 50 for the size of each sample.
   - An empty list `sample_means` is created to store the mean of each sample.

7. **Generate Samples and Calculate Means**:  
   A loop runs 1000 times, each time selecting a random sample of size 50 from the `scores` column using `np.random.choice()`. The mean of each sample is calculated and appended to the `sample_means` list.

8. **Plot Distribution of Sample Means**:  
   The distribution of sample means is visualized using Seaborn's `histplot()` with a KDE (kernel density estimate) to show the smooth distribution. The plot shows how the sample means form a normal distribution according to the Central Limit Theorem.

9. **Calculate and Print Sampling Mean**:  
   The mean of the sample means is calculated using `np.mean()` and printed.

10. **Calculate and Print Actual Mean**:  
    The actual mean of the 'Score' column is calculated using `np.mean(scores)` and printed.

11. **Compare the Means**:  
    The difference between the sampling mean and the actual mean is calculated and printed to show how close the sampling distribution mean is to the population mean.


