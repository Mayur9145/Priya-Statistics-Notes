
## 1. Write a Python code snippet to generate a histogram of 10,000 samples from a normal distribution with mean 0 and standard deviation 1. Explain why the shape of the histogram resembles a bell curve.



```python

import numpy as np
import matplotlib.pyplot as plt

mean = 0
std_dev = 1
num_samples = 10000

data = np.random.normal(mean, std_dev, num_samples)

plt.hist(data, bins=50, density=True, alpha=0.6, color='b')

plt.title('Histogram of 10,000 Samples from Normal Distribution')
plt.xlabel('Value')
plt.ylabel('Density')

plt.show()

````

[colab](https://colab.research.google.com/drive/1RiEyJpnENBm-LAbaxyy9sBuCWfCdvTTl#scrollTo=u8bnfaI-ESUV)


### The above is the colab file link  for question 1


```python
import numpy as np
import matplotlib.pyplot as plt

# Define the mean and standard deviation for the normal distribution
mean = 0          # Mean of the distribution
std_dev = 1       # Standard deviation of the distribution
num_samples = 10000  # Number of samples to generate

# Generate random samples from a normal (Gaussian) distribution
# np.random.normal takes in the mean, standard deviation, and number of samples
data = np.random.normal(mean, std_dev, num_samples)

# Create a histogram to visualize the distribution of the generated data
# bins=50 divides the data into 50 intervals
# density=True normalizes the histogram so that the area under it sums to 1
# alpha=0.6 makes the histogram semi-transparent
# color='b' sets the color of the bars to blue
plt.hist(data, bins=50, density=True, alpha=0.6, color='b')

# Add a title and labels for the axes to make the plot more informative
plt.title('Histogram of 10,000 Samples from Normal Distribution')  # Title of the plot
plt.xlabel('Value')  # Label for the x-axis representing the values of the samples
plt.ylabel('Density')  # Label for the y-axis representing the density (normalized frequency)

# Display the plot to the screen
plt.show()
```

##  2. Use Python to load the dataset (score.csv) and plot the distribution of the 'Income' column. Describe its shape and explain why it is not normally distributed.



```python
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
from google.colab import files

# Prompt the user to upload a file
uploaded = files.upload()

# Assuming the uploaded file is score.csv
df = pd.read_csv(list(uploaded.keys())[0])

# Plot the distribution of the 'Income' column
plt.figure(figsize=(10, 6))
sns.histplot(df['Income'], bins=30, kde=True)
plt.title('Distribution of Income')
plt.xlabel('Income')
plt.ylabel('Frequency')
plt.show()

```
[colab](https://colab.research.google.com/drive/1_j3v48iCkoxZac7ghFYozP2RWR4UqFbK#scrollTo=z7doCJ7nGPOT)



### The above is the colab file link for question 2


```python
# Import necessary libraries
import pandas as pd  # For data manipulation and analysis
import matplotlib.pyplot as plt  # For creating static, animated, and interactive visualizations
import seaborn as sns  # Built on top of matplotlib, seaborn provides a high-level interface for drawing attractive statistical graphics
from google.colab import files  # Used to interact with the file system in Google Colab

# Prompt the user to upload a file
uploaded = files.upload()  # This will open a dialog box allowing the user to upload a file from their local system.

# Read the uploaded CSV file into a DataFrame
# list(uploaded.keys())[0] gets the filename of the uploaded file (since files.upload() returns a dictionary)
df = pd.read_csv(list(uploaded.keys())[0])  # This reads the CSV file into a Pandas DataFrame. 'df' now contains the dataset.

# Create a plot to show the distribution of the 'Income' column
plt.figure(figsize=(10, 6))  # Sets the size of the plot (width, height in inches)

# Use seaborn's histplot to plot the distribution of the 'Income' column with a Kernel Density Estimate (kde=True)
sns.histplot(df['Income'], bins=30, kde=True)  # 'bins=30' specifies the number of bins for the histogram, kde=True adds the KDE line

# Add title and labels to the plot
plt.title('Distribution of Income')  # Title of the plot
plt.xlabel('Income')  # Label for the x-axis
plt.ylabel('Frequency')  # Label for the y-axis

# Display the plot
plt.show()  # This will output the plot in the current environment (Google Colab in this case)
```




