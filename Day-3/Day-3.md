# Measures of Dispersion

Measures of dispersion describe the spread or variability in a dataset. Below are some common measures of dispersion with examples.

## 1. **Range**
The difference between the maximum and minimum values in a dataset.

### Formula:
\[ \text{Range} = \text{Max} - \text{Min} \]

### Example:
For the dataset [3, 7, 8, 12, 15]:
\[
\text{Range} = 15 - 3 = 12
\]

---

## 2. **Variance**
The average of the squared differences from the mean. 

### Formula:
\[
\text{Variance} (\sigma^2) = \frac{\sum (x_i - \mu)^2}{n}
\]
Where \(x_i\) is each data point, \(\mu\) is the mean, and \(n\) is the number of data points.

### Example:
For the dataset [4, 6, 8], the mean is 6:
\[
\text{Variance} = \frac{(4-6)^2 + (6-6)^2 + (8-6)^2}{3} = \frac{4 + 0 + 4}{3} = 2.67
\]

---

## 3. **Standard Deviation**
The square root of variance, representing the average distance of each data point from the mean.

### Formula:
\[
\text{Standard Deviation} (\sigma) = \sqrt{\frac{\sum (x_i - \mu)^2}{n}}
\]

### Example:
For the dataset [4, 6, 8]:
\[
\text{Standard Deviation} = \sqrt{2.67} = 1.63
\]

---

## 4. **Interquartile Range (IQR)**
The difference between the third quartile (Q3) and the first quartile (Q1). It measures the spread of the middle 50% of data.

### Formula:
\[
\text{IQR} = Q3 - Q1
\]

### Example:
For the dataset [5, 7, 9, 10, 12, 15, 18], Q1 = 7, Q3 = 15:
\[
\text{IQR} = 15 - 7 = 8
\]

---

## 5. **Mean Absolute Deviation (MAD)**
The average of the absolute differences between each data point and the mean.

### Formula:
\[
\text{MAD} = \frac{\sum |x_i - \mu|}{n}
\]

### Example:
For the dataset [4, 6, 8], the mean is 6:
\[
\text{MAD} = \frac{|4 - 6| + |6 - 6| + |8 - 6|}{3} = \frac{2 + 0 + 2}{3} = 1.33
\]

---

## 6. **Coefficient of Variation (CV)**
The ratio of the standard deviation to the mean, often expressed as a percentage.

### Formula:
\[
\text{CV} = \frac{\sigma}{\mu} \times 100
\]

### Example:
For a dataset with a mean of 50 and a standard deviation of 5:
\[
\text{CV} = \frac{5}{50} \times 100 = 10\%
\]

# Empirical Formula in Statistics

## Formula
The empirical formula in statistics refers to the computation of the empirical rule, which states that for a normal distribution:
- 68% of data lies within 1 standard deviation (σ) from the mean (μ)
- 95% of data lies within 2 standard deviations (σ) from the mean (μ)
- 99.7% of data lies within 3 standard deviations (σ) from the mean (μ)

### Formula:
```math
μ ± σ = 68\%
μ ± 2σ = 95\%
μ ± 3σ = 99.7\%



# Interquartile Range (IQR) in Statistics

## Definition
The **Interquartile Range (IQR)** is a measure of statistical dispersion, which is the spread of the middle 50% of a dataset. It is calculated as the difference between the third quartile (Q3) and the first quartile (Q1).

IQR = Q3 - Q1

Where:
- **Q1**: The first quartile (25th percentile)
- **Q3**: The third quartile (75th percentile)

## Example Calculation

Consider the following dataset:
