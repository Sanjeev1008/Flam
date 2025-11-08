# Flam
Research and Development Assignment

# Parameter Estimation for a Parametric Curve Model

## 📘 Overview
This project focuses on estimating the parameters **θ (theta)**, **M**, and **X** in a nonlinear **parametric curve model** using numerical optimization.  
The model equations are given by:

\[
x(t) = t\cos(\theta) - e^{M|t|}\sin(0.3t)\sin(\theta) + X
\]
\[
y(t) = 42 + t\sin(\theta) + e^{M|t|}\sin(0.3t)\cos(\theta)
\]

The aim is to find parameter values that best fit the dataset \((t_i, x_i, y_i)\) by minimizing the total squared error between observed and predicted values.

---

## 🎯 Objective
To estimate parameters \(\theta, M, X\) that minimize:
\[
E(\theta, M, X) = \sum_i \big[(x_i - \hat{x}_i)^2 + (y_i - \hat{y}_i)^2\big]
\]
where \(\hat{x}_i, \hat{y}_i\) are the predicted coordinates from the model.

---

## 📂 Project Structure
```bash
Parametric-Curve-Estimation/
-- xy_data.csv # Input dataset file
-- Assignment.py # Python implementation
-- OUT_res.csv # Output file with fitted curve values
-- output.png # Plot of observed vs fitted data
-- report.tex # Complete LaTeX report

```


---

## ⚙️ Requirements
Make sure you have Python 3.8 or above installed.

Install required dependencies:
```bash

pip install numpy pandas matplotlib scipy

```
##execution
```bash
python parametric_fit.py
```

### Sample Output
Theta (°): 12.684532
M:         0.01483257
X:         22.946281
Sum of Squared Errors: 1.347e-03

