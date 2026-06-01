# Real Estate Valuation Dataset

## Introduction and problem statement
The **Real Estate Valuation Dataset** is a multivariate dataset containing historical market data collected from the Sindian District in New Taipei City, Taiwan. Donated in August 2018, the dataset was originally utilized by *I. Yeh and Tzu-Kuang Hsu (2018)* to build predictive models using case-based reasoning and comparative approaches.

The core problem statement belongs to the business and financial domain, specifically framed as a **regression task**. The objective is to accurately estimate and predict property valuations based on geographical, temporal, and neighborhood attributes. Accurate automated real estate valuation helps buyers, sellers, and financial institutions appraise property values efficiently without relying solely on manual, time-consuming on-site appraisals. In the introductory literature, the dataset of $414$ instances was randomly partitioned into a training set ($\frac{2}{3}$ of the samples) and a testing set ($\frac{1}{3}$ of the samples) to evaluate predictive performance.

---

## Contained attributes
The dataset consists of $414$ observations with $6$ predictive features, an indexing attribute, and a target variable. There are no missing values in this dataset. The attributes are detailed below:

* **No**: Patient or record index identifier (Integer; not used as a predictive feature).
* **X1 transaction date**: The date when the real estate transaction occurred, represented as a continuous decimal year (e.g., $2013.250 = \text{March 2013}$, $2013.500 = \text{June 2013}$, etc.).
* **X2 house age**: The age of the house (Continuous; measured in $\text{years}$).
* **X3 distance to the nearest MRT station**: The geodesic or transit distance to the nearest Mass Rapid Transit station (Continuous; measured in $\text{meters}$).
* **X4 number of convenience stores**: The total count of convenience stores accessible within a walking distance living circle (Integer).
* **X5 latitude**: The geographic latitude coordinate of the property (Continuous; measured in $\text{degrees}$).
* **X6 longitude**: The geographic longitude coordinate of the property (Continuous; measured in $\text{degrees}$).

---

## Potential targets
The target variable to be predicted by regression models is the unit price of the property:

* **Y house price of unit area**: The continuous valuation of the property per unit area.
    * **Unit**: $10,000\text{ New Taiwan Dollar/Ping}$
    * *Note on local units*: A "Ping" is a traditional Taiwanese unit of area where $1\text{ Ping} = 3.3\text{ m}^2$.