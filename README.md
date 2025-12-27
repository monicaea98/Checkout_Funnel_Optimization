# 🧪 A/B Test Analysis – Checkout Funnel Optimization

This project analyzes the performance of a **new checkout funnel with an improved recommendation system** using an A/B testing framework. The goal is to evaluate whether the new funnel design improves user conversion across key stages of the purchase process.

---

## 🎯 Study Objectives

An A/B test was conducted to compare two user groups:

* **Group A** — Control group (current checkout funnel)
* **Group B** — Experimental group (new funnel with enhanced recommendations)

The main objective is to determine whether the new funnel leads to higher conversion rates across the following stages:

* **Login**
* **Product Page View** (`product_page`)
* **Add to Cart** (`product_cart`)
* **Purchase Completion** (`purchase`)

The experiment assumes that, within **14 days after registration**, users in **Group B** should show at least a **10% increase in conversion** at each funnel stage compared to Group A.

Before analyzing the results, the experiment setup was validated to ensure:

* Correct group assignment
* Data completeness and consistency
* Absence of anomalies that could bias the results

---

## 📊 Methodology

The analysis includes:

* Data cleaning and validation of user events
* Construction of conversion funnels for both groups
* Comparison of conversion rates at each funnel stage
* Statistical evaluation of differences between Group A and Group B
* Interpretation of results with a product-focused perspective

---

## 📈 Key Results

* The **new funnel (Group B)** showed an **improvement in the intermediate conversion rate** from `product_page` to `product_cart`.
* This suggests that the improved recommendation system may enhance **user engagement and intent** at earlier stages of the funnel.
* However, **no improvement was observed in the final purchase conversion rate**, which is the primary business objective.

---

## 🧠 Conclusion

Although the new checkout interface improves conversion at intermediate stages, it **does not lead to a higher purchase completion rate**. As a result, there is **insufficient evidence to justify permanently implementing the new funnel**.

---

## 📌 Recommendations

* Review the **event tracking system**, particularly the transition from `product_cart` to `purchase`, to ensure accurate data collection.
* Conduct a **new controlled A/B test** with a fully validated and consistent data pipeline.
* Explore additional optimizations focused on reducing friction in the **final purchase stage**.

---

## 🛠️ Tools & Technologies

* 🐍 **Python**
* 📊 **Pandas & NumPy** — data preprocessing and funnel construction
* 📈 **Matplotlib / Seaborn** — visualization of funnel performance
* 🧮 **Statistical Testing** — comparison of conversion rates
* 📘 **Jupyter Notebook** — interactive analysis
