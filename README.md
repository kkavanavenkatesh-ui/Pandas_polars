# Polars vs Pandas Benchmark

Hey! This repository contains a quick project comparing **Pandas** and **Polars** to see how they stack up in terms of speed and memory usage. 

I ran these tests using a synthetic dataset with **1 million rows** in Google Colab to see how both libraries handle common data tasks.

---

## What's in this project?
I tested both libraries on 6 core data manipulation tasks:
1. **Loading data** from a CSV file.
2. **Filtering rows** based on a numerical condition.
3. **Selecting columns** from the dataset.
4. **Grouping and aggregating** (finding means and sums by category).
5. **Joining** the main dataset with a smaller lookup table.
6. **Sorting and transforming** (sorting by values and calculating a new column).

---

## Tools Used
* Python
* Pandas & Polars
* NumPy (to generate the test data)
* Matplotlib & Seaborn (for plotting the graphs)
* `tracemalloc` (to track memory usage)

---

## Results Summary

| Operation | Pandas Time (s) | Polars Time (s) | Pandas Memory (MB) | Polars Memory (MB) |
| :--- | :--- | :--- | :--- | :--- |
| **Load Dataset** | *[Your data here]* | *[Your data here]* | *[Your data here]* | *[Your data here]* |
| **Filter Rows** | *[Your data here]* | *[Your data here]* | *[Your data here]* | *[Your data here]* |
| **Select Columns** | *[Your data here]* | *[Your data here]* | *[Your data here]* | *[Your data here]* |
| **Group & Aggregate** | *[Your data here]* | *[Your data here]* | *[Your data here]* | *[Your data here]* |
| **Join Datasets** | *[Your data here]* | *[Your data here]* | *[Your data here]* | *[Your data here]* |
| **Sort & Transform** | *[Your data here]* | *[Your data here]* | *[Your data here]* | *[Your data here]* |

---

## What I Learned / Takeaways
* **Polars is way faster** for most operations, especially heavy lifting like sorting, grouping, and reading files. This is mostly because it uses multi-threading out of the box and is built on Apache Arrow.
* **Pandas is still great** for small datasets, quick exploratory work, or when working with older libraries that expect pandas DataFrames. But for big data pipelines, Polars is definitely the better choice.

---

## How to run it
1. Open the `.ipynb` notebook file in Google Colab.
2. Run the cells from top to bottom to regenerate the data and check the output tables/charts.
