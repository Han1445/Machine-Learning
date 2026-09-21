In this lab assignment, I preprocessed the Penguins dataset through these steps:

Tasks 1 & 2 (Cleaning & Missing Values): Cleaned body_mass_g to float64 and tested all four strategies: Row Deletion, Mean, Median, and Mode Imputation. Combining Median (for numbers) and Mode (for text) was the best choice because it preserved all 1,000 rows without letting outliers distort the data.

Task3(Outliers): Detected extreme values using the IQR method and handled them to prevent skewed results.

Task4(Scaling): Applied Min-Max Scaling and Z-score Standardization.

Task5(PCA): Applied PCA for dimensionality reduction and checked the explained variance ratio.