# 🎵 Gaana Songs Dataset Analysis

This project focuses on analyzing a dataset containing songs from **Gaana**. It involves data cleaning, transformation, and exploratory analysis to understand patterns related to songs, singers, and languages.

---

## 📂 Dataset Description

The dataset used in this project is located at:

Gaana/songs.csv


### 📝 Columns in Dataset:
| Column Name | Description |
|-------------|-------------|
| `name`      | Name of the song |
| `singer`    | Singer(s) of the song (multiple singers separated by `|`) |
| `singer_id` | Unique ID(s) of the singer(s) (separated by `|`) |
| `duration`  | Song duration in time format (`MM:SS` or `HH:MM:SS`) |
| `link`      | Unique link to the song on Gaana (used for deduplication) |
| `language`  | Language of the song |

---

## 🔧 Key Steps Performed

1. **Data Loading**  
    Loaded dataset using `pandas`.

2. **Data Cleaning**  
    - Removed duplicate entries based on:
        - `link`
        - Combination of `name`, `singer`, `singer_id`, and `duration`
    - Converted song duration into seconds:
        - Added a new column `duration_in_sec` for easier analysis.

3. **Exploratory Data Analysis (EDA)**  
    - Examined overall data distribution and unique counts.
    - Explored the most common languages in the dataset.
    - Identified frequently occurring singers and popular song durations.
    - Checked correlations and potential groupings based on singer popularity and song duration.

---

## 🐍 Tech Stack & Libraries

- Python
- pandas
- numpy
- seaborn
- matplotlib.pyplot

---

## 📂 Project Structure

- `Gaana.ipynb` → Jupyter Notebook containing the full analysis
- `songs.csv` → Dataset 



---

## 🚀 How to Run

1. Open the notebook `Gaana.ipynb` using **Google Colab** or **Jupyter Notebook**.
2. Make sure `pandas` and `numpy` are installed:
```bash
pip install pandas numpy seaborn matplotlib
```
3. Adjust the dataset path if required.
4. Run cells step by step.

## 💡 Project Purpose
This project serves as a data analysis practice to enhance data wrangling, cleansing, and exploratory analysis skills using Python.

## 🙌 Contributions & Feedback
This is a personal learning project.

Feel free to explore, fork, or suggest improvements!
