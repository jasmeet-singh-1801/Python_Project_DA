
#### 📊 Project Overview

This project explores, cleans, and analyzes Airbnb listing data to uncover insights about property prices, guest reviews, host activity, amenities, and safety features. Through structured data preprocessing and visualization techniques, the notebook delivers actionable insights on what factors influence Airbnb pricing and popularity.

---

### 🧠 Key Skills Demonstrated

* **Data Cleaning & Wrangling**: Regex-based string cleaning, handling missing values, type conversions.
* **EDA (Exploratory Data Analysis)**: Univariate and multivariate analysis using histograms, scatter plots, box plots.
* **Feature Engineering**: Extraction and transformation of complex fields like `amenities`, `room_type`, and `host name`.
* **Data Visualization**: Matplotlib and Seaborn used to visualize relationships between variables.
* **Insight Derivation**: Deep-dive into how location, room type, reviews, and safety features influence price and ratings.

---

### 📁 Dataset Used

* The dataset is a CSV file containing **Airbnb listings** with columns like:

  * `price`, `rating`, `reviews`, `host_id`, `amenities`, `room_type`, `location`, etc.

---

### 📌 Project Structure

#### 🔹 1. Data Cleaning

* **Price Column**: Cleaned to remove symbols (`₹`, commas, text like "per night").
* **Rating**: Converted "New" entries to `NaN` and casted to float.
* **Reviews**: Non-numeric reviews parsed and missing values imputed with 0.
* **Host ID**: Ensured appropriate data type.
* **Dropped unnecessary columns** to reduce noise.
* **Handled missing values** systematically.

#### 🔹 2. Feature Extraction

* **Host Name**: Extracted and analyzed frequency of listings per host.
* **Property Type & Room Type**: Cleaned inconsistent naming, grouped similar entries.
* **Amenities**: Parsed as lists and analyzed frequency of amenities.
* **Safety Rules**: Cleaned and visualized presence of safety features.

#### 🔹 3. Exploratory Data Analysis (EDA)

* **Price Distribution**: Histogram and box plots used.
* **Price vs Room Type**: Comparison of average prices across room types.
* **Price vs Reviews**: Analyzed relationship between number of reviews and pricing.
* **Guest Capacity & Bedrooms**: Impact on price analyzed via scatter plots.
* **Top Cities by Listing**: Location-based pricing visualized for top contributors.
* **Correlation Matrix**: Heatmap showing interrelations among numerical variables.

#### 🔹 4. In-Depth Analysis

* **Amenities vs Price**: Average price per common amenity.
* **Safety Features**: Evaluated importance on both price and rating.
* **Listings per Host**: Identified patterns for hosts with multiple listings.

#### 🔹 5. Data Export

* Cleaned and transformed dataframe exported for future modeling or dashboarding.

---

### 📌 Notable Insights

* **Room Type** plays a crucial role in price variation — entire homes cost more.
* **Safety Features** are positively associated with both higher prices and better ratings.
* Hosts with **multiple listings** often provide lower average pricing.
* **Top amenities** like Wi-Fi, Kitchen, and TV dominate listings.
* Locations in **urban centers** are priced significantly higher than rural areas.

---

### 🧰 Technologies Used

| Tool         | Purpose                   |
| ------------ | ------------------------- |
| `pandas`     | Data manipulation         |
| `numpy`      | Numerical operations      |
| `matplotlib` | Visualization             |
| `seaborn`    | Statistical plotting      |
| `regex`      | Text cleaning and parsing |

---

### ✅ Next Steps

* Build a **pricing prediction model** using features like reviews, safety, and amenities.
* Create a **dashboard** using Power BI or Tableau for stakeholder insights.
* Integrate **geolocation mapping** for spatial analysis using Folium/Plotly.

---

### 📎 File Output

* ✔ Cleaned DataFrame exported to CSV (`cleaned_airbnb_data.csv`)
* ✔ Notebook provides visual and statistical insights for decision-making.


