# Measures of Central Tendency

## 1. Mean
The mean is the sum of all values divided by the number of values.

**Formula**:
\[
\text{Mean} = \frac{\sum x}{n}
\]
**Example**:
If the values are: 10, 15, 20, 25, 30
\[
\text{Mean} = \frac{10 + 15 + 20 + 25 + 30}{5} = 20
\]

## 2. Median
The median is the middle value in a dataset when arranged in ascending or descending order.

**Example**:
If the values are: 10, 15, 20, 25, 30  
The median is **20** (middle value).

If there are an even number of values:  
Values: 10, 15, 20, 25  
The median is \(\frac{15 + 20}{2} = 17.5\).

## 3. Mode
The mode is the value that appears most frequently in a dataset.

**Example**:
If the values are: 10, 15, 20, 20, 30  
The mode is **20** (since it appears twice).



### Population vs. Sample

#### Population:
A **population** refers to the entire group of individuals, items, or data from which information is required or on which conclusions need to be drawn. It includes every possible subject that fits a particular criterion.

- **Example**: 
    - In a study about the average height of adults in the United States, the **population** would be **all adults in the United States**.

#### Sample:
A **sample** is a subset of the population, selected for analysis, which represents the population. It's used when studying the entire population is impractical due to time, cost, or other constraints.

- **Example**: 
    - In the same study, instead of measuring the height of all adults in the U.S., you might select **a sample of 1,000 adults** from various regions to estimate the average height.


# Variance and Standard Deviation

## Variance
Variance measures how spread out the numbers in a data set are. It is calculated as the average of the squared differences from the mean.

### Formula:
\[
\text{Variance} (\sigma^2) = \frac{\sum (x_i - \mu)^2}{N}
\]
Where:
- \(x_i\) = each value in the dataset
- \(\mu\) = mean of the dataset
- \(N\) = number of values in the dataset

### Example:
Let's say we have the following data points: 3, 7, 7, 19, 24.

1. Calculate the mean:
   \[
   \mu = \frac{3 + 7 + 7 + 19 + 24}{5} = 12
   \]

2. Find the squared differences from the mean:
   \[
   (3 - 12)^2 = 81,\quad (7 - 12)^2 = 25,\quad (7 - 12)^2 = 25,\quad (19 - 12)^2 = 49,\quad (24 - 12)^2 = 144
   \]

3. Calculate the variance:
   \[
   \text{Variance} = \frac{81 + 25 + 25 + 49 + 144}{5} = \frac{324}{5} = 64.8
   \]

## Standard Deviation
Standard deviation is the square root of the variance. It gives a measure of the spread of the data in the same units as the data.

### Formula:
\[
\text{Standard Deviation} (\sigma) = \sqrt{\text{Variance}}
\]

### Example:
Using the variance calculated above (64.8):
\[
\sigma = \sqrt{64.8} \approx 8.05
\]

Thus, the standard deviation of the data set is approximately 8.05.

