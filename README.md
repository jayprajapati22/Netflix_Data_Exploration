# Netflix_Data_Exploration
This project analyzes Netflix's dataset to explore trends in genres, content types, and other attributes. It processes data, splits multiple genres per entry, counts their occurrences, and displays insights on the most common genres.

## Dataset
- **Source**: Netflix Titles Dataset
- **File Used**: `netflix_titles.csv`
- **Total Entries**: 8,807
- **Columns**: 12 (including `show_id`, `type`, `title`, `director`, `cast`, `country`, `date_added`, `release_year`, `rating`, `duration`, `listed_in`, `description`)

## Exploratory Data Analysis (EDA)

### Basic Information
- Displayed column names, data types, and dataset summary.
- Checked for missing values in each column.
- Counted unique values in categorical columns.

### Data Cleaning & Transformation
- Created new columns: 
  - `new_title`: Stores the length of each title.
  - `short`: Simplifies the `type` column (Movie → M, TV Show → TV).
  - `sorted_list`: Mapped `Movie` to `M`, leaving `TV Show` as NaN.
  - `now`: Counts the number of words in each description.
- Replaced missing values where applicable.

### Data Insights
- Counted unique categories in `type` and `country` columns.
- Analyzed the distribution of ratings.
- Filtered data for specific conditions, e.g., shows released after 2023 (resulted in an empty dataset).

## Visualizations
- Used `matplotlib` and `seaborn` for graphical representation.
- Created bar charts and histograms to visualize:
  - Distribution of content types (Movies vs. TV Shows).
  - Most common ratings and their frequency.
  - Trends in content release years.

## Results & Key Findings
- Netflix has more movies (6,131) than TV shows (2,676).
- The most common rating is `TV-MA` (3,207 titles).
- `release_year` data shows a significant increase in content production after 2010.
- There are 748 unique countries in the dataset, indicating diverse content origins.
- Missing data is prevalent in `director`, `cast`, and `country` columns.

## Technologies Used
- **Python**
- **Pandas** for data manipulation
- **Matplotlib & Seaborn** for visualization

## Future Improvements
- Handle missing values more effectively.
- Perform deeper analysis on genres and content trends.
- Use machine learning for recommendations based on content metadata.

