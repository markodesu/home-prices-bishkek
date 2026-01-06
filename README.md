## 📍 Project Background

In **2023**, my teammate and I attended the **Machine Learning Bootcamp** organized by **IncubAsia Lab**, hosted in **Naryn**.
The bootcamp focused on applying **machine learning and data analysis techniques** to real-world datasets.

As part of the program, we analyzed **housing market data from Bishkek** to answer the following question:

> **Which factors have the strongest influence on house prices in Bishkek?**

This project focuses on **exploratory data analysis (EDA)** using visualization and correlation analysis as a foundation for future machine learning models.

---

## 📊 Dataset Overview

The dataset contains approximately **10,000 real estate listings** from Bishkek.
Each row represents a single housing advertisement.

### Key Numerical Features

* `price` — house price
* `square` — total area (m²)
* `rooms` — number of rooms
* `floor` — floor number
* `year` — year of construction

Pearson correlation was computed using:

```python
df[['price', 'square', 'rooms', 'floor', 'year']].corr()
```
<Figure size 640x480 with 1 Axes><img width="619" height="413" alt="image" src="https://github.com/user-attachments/assets/07e3e2f9-82db-4844-aa70-c15b560fbb3f" />

---

## 📈 Distribution of House Prices

**Histogram: Price Distribution**

The distribution of housing prices is **right-skewed**:

* Most listings fall into a moderate price range
* A small number of houses have extremely high prices
* These premium properties form a long tail

This indicates market inequality and suggests that the **median price** is often more informative than the mean price.

---

## 📐 Area and House Prices

**Scatter Plot: Square Meters vs Price**

There is a **strong positive relationship** between total area and price:

* Larger houses consistently cost more
* Price variance increases for very large properties

**Correlation coefficient:**

```text
corr(price, square) ≈ 0.82
```

➡️ **Area is the most influential factor in Bishkek housing prices.**

---

## 🛏️ Number of Rooms vs Price

**Scatter Plot: Rooms vs Price**

The number of rooms shows a **moderate positive correlation** with price:

* More rooms generally mean higher prices
* Significant price variation exists within the same room count

**Correlation coefficient:**

```text
corr(price, rooms) ≈ 0.61
```

Room count alone does not capture layout quality or location effects.

---

## 🏗️ Year of Construction and Price

**Histogram: Year Built**
**Scatter Plot: Year Built vs Price**

Newer buildings tend to have higher prices, while older houses cluster at lower price ranges.

**Correlation coefficient:**

```text
corr(price, year) ≈ 0.47
```

Building age has a moderate influence and interacts strongly with location and condition.
<Figure size 800x400 with 1 Axes><img width="721" height="393" alt="image" src="https://github.com/user-attachments/assets/4090290e-64b4-4382-b08f-7420bd65e9f6" />
<Figure size 640x480 with 1 Axes><img width="597" height="432" alt="image" src="https://github.com/user-attachments/assets/e58197fb-6ab4-4717-b967-ab0d4b0d8585" />

---

## 🏢 Floor Number vs Price

**Scatter Plot: Floor vs Price**

The relationship between floor number and price is weak.

**Correlation coefficient:**

```text
corr(price, floor) ≈ 0.12
```

Floor number alone does not significantly affect house prices.

---

## 🔍 Correlation Summary

| Feature        | Correlation | Impact         |
| -------------- | ----------- | -------------- |
| 🟦 Square (m²) | ~0.82       | 🔥 Very strong |
| 🛏️ Rooms      | ~0.61       | ⚡ Moderate     |
| 🏗️ Year Built | ~0.47       | ⚡ Moderate     |
| 🏢 Floor       | ~0.12       | 💤 Weak        |

---

## 🧠 Key Insights

* Housing prices in Bishkek are primarily driven by **property size**
* **Newer constructions** are generally more expensive
* **Room count** partially explains price variation
* **Floor number** has minimal standalone impact

<Figure size 1500x1500 with 7 Axes><img width="1489" height="1490" alt="image" src="https://github.com/user-attachments/assets/f520c0ff-99d9-411a-a2aa-e239c9a13612" />
---

## ✅ Conclusion

This project demonstrates the importance of **exploratory data analysis (EDA)** in understanding real-world housing markets.

By combining:

* histograms for distribution analysis
* scatter plots for feature relationships
* correlation coefficients for validation

we identified the main factors influencing housing prices in Bishkek.

This analysis provides a strong foundation for future work, including **predictive modeling** and **machine learning applications**.

---

## 🎓 Bootcamp Experience

This project was completed during the **Machine Learning Bootcamp (2023)** organized by **IncubAsia Lab** and hosted in **Naryn**.
The bootcamp emphasized **practical learning**, **teamwork**, and **real-world data analysis**.

⭐ See the notebook in this repository for full implementation details.

---

