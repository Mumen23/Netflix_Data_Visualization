# Netflix Data Analysis

## Overview
This project analyzes Netflix movies and TV shows using Python and the Pandas, Seaborn, and Matplotlib libraries. The dataset is cleaned and visualized to extract meaningful insights, such as the most watched genres and the distribution of ratings.

## Prerequisites
Ensure you have Python installed on your system. You can download it from [Python.org](https://www.python.org/downloads/).

### Required Python Libraries
You need the following Python libraries to run the script:
- pandas
- seaborn
- matplotlib

Install them using the following command:
```bash
pip install pandas seaborn matplotlib
```

## Dataset
The script uses a dataset named `netflix_data.csv`, which contains details about Netflix movies and TV shows, including:
- `show_id` - Unique identifier for each show
- `type` - Whether the content is a Movie or a TV Show
- `title` - Title of the show
- `director` - Name of the director
- `cast` - List of actors
- `country` - Country of production
- `date_added` - Date when the show was added to Netflix
- `release_year` - Year of release
- `rating` - Audience rating (e.g., PG-13, R, etc.)
- `duration` - Duration of the movie or number of seasons for a TV show
- `listed_in` - Genre(s) of the content
- `description` - Short summary of the show

## How to Use
### Running the Script
1. Download the dataset `netflix_data.csv` and place it in the same directory as `script.py`.
2. Run the script using:
   ```bash
   python script.py
   ```
3. The script will:
   - Load and clean the dataset (remove missing values)
   - Display summary statistics
   - Generate visualizations for the most watched genres and ratings distribution
   - Save the cleaned dataset as `Netflix_shows_movies.csv`

### Expected Outputs
1. **Summary Statistics:** Basic details about the dataset will be printed.
2. **Genre Analysis:** A bar chart showing the top 10 most watched genres.
3. **Ratings Distribution:** A histogram displaying the distribution of content ratings.
4. **Cleaned Dataset:** The script saves a cleaned version of the dataset as `Netflix_shows_movies.csv`.

## Troubleshooting
- **ModuleNotFoundError:** If you get an error about missing libraries, install them using `pip install pandas seaborn matplotlib`.
- **KeyError: 'genre':** If you encounter an error related to the 'genre' column, ensure you are using the updated script that references `listed_in` instead.
- **FileNotFoundError:** Make sure `netflix_data.csv` is in the same directory as the script.

