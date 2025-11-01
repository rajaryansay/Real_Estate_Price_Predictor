🚀 Project Workflow
✅ 1. Data Cleaning

Removed unnecessary columns (area_type, society, availability, balcony)

Handled missing values

Converted bedroom text field (2 BHK, 3 Bedroom) → numeric bhk

Converted total_sqft ranges like 1200-1500 to numeric average

✅ 2. Feature Engineering

Added price_per_sqft feature

Reduced high-cardinality location column (grouped rare locations as other)

One-hot encoding on location

✅ 3. Outlier Removal

Removed outliers based on:

Minimum sqft per BHK rule (total_sqft/bhk < 300)

Price per sqft deviation

Bathroom > Bedrooms + 2

✅ 4. Model Building

Train-test split

Linear Regression Model

Cross-validation
