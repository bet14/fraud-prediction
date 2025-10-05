**Explanation (for GitHub README or code comment)**

This script analyzes whether the numerical data in the columns **`count`**, **`registered`**, and **`casual`** from the file `train.csv` follow **Benford’s Law** — a statistical principle stating that in many naturally occurring datasets, smaller digits appear more frequently as the first digit.

**How it works:**

1. Imports necessary libraries (`csv`, `collections`, `math`, `matplotlib`).
2. Reads `train.csv` and counts the first digit of each number in the three specified columns.
3. Excludes zeros since Benford’s Law applies to non-zero leading digits (1–9).
4. Normalizes the counts to obtain probability distributions.
5. Generates Benford’s expected distribution using the formula `log10(1 + 1/digit)`.
6. Plots and compares the dataset’s first-digit distribution with the theoretical Benford distribution.
7. Saves the resulting plot as `Benford1.png`.

**Purpose:**
Used for **data integrity checks** or **fraud detection**, since significant deviations from Benford’s Law may indicate anomalies or artificial manipulation in datasets.
