# Movie Studio Data Analysis
## Project Overview
This project focuses on providing data-driven insights to a new movie studio, guiding their content creation strategy to maximize box office success. By analyzing historical movie data, we aim to identify key characteristics of films that perform well financially.

## Business Problem
My company is venturing into original video content with a new movie studio but lacks experience in film production. The objective is to explore current box office trends to understand what types of films are most successful and translate these findings into actionable recommendations for the studio head.

## Data Sources
The analysis leverages data from two primary sources:

[Box Office Mojo](bom.movie_gross.csv.gz): Provides domestic and foreign gross revenue figures for movies.

[IMDB](im.db.zip): A SQLite database containing movie metadata such as titles, release years, genres, average ratings, and number of votes. (Specifically, movie_basics and movie_ratings tables are used).

## Methodology
Data Acquisition: Loaded Box Office Mojo data from a compressed CSV and extracted/connected to the IMDB SQLite database.

### Data Preparation:

- Merged IMDB's movie_basics and movie_ratings tables on movie_id.

- Cleaned and converted gross revenue columns to numeric types, handling missing values by filling with zero.

- Cleaned movie titles for merging across datasets by converting to lowercase and removing non-alphanumeric characters.

- Merged the cleaned Box Office Mojo data with the combined IMDB data, primarily on cleaned movie titles.

- Handled missing genres and filtered out movies with zero total gross.

### Exploratory Data Analysis (EDA):

- Analyzed average worldwide gross by genre to identify top-performing categories.

- Investigated the relationship between audience ratings, number of votes, and total gross, focusing on movies with a significant number of votes.

- Examined correlations between key financial and audience metrics.

## Business Recommendations: 
Formulated three concrete, data-backed recommendations for the movie studio based on the analytical findings.

### Key Findings & Recommendations
My analysis revealed several critical insights:

Genre Dominance: Adventure, Action, and Sci-Fi genres consistently show the highest average worldwide gross.

#### Recommendation 1: 
Prioritize the development of films within Adventure, Action, and Sci-Fi genres to maximize box office potential.

Audience Engagement is Key: A high number of audience votes (indicating broad engagement) is a strong predictor of higher worldwide gross, even more so than just a high average rating.

#### Recommendation 2: 
Invest in films that can generate widespread interest and encourage broad audience participation and discussion.

Broad Appeal Wins: The highest-grossing films often resonate with a very wide audience, suggesting the importance of universal themes.

#### Recommendation 3: 
Focus on producing movies with broad audience appeal and themes that can attract a diverse and large demographic.

### Visualizations
The project includes several visualizations to support the findings:

#### Bar Chart: [Top 10 Movie Genres by Average Worldwide Gross(.PNG)](WorlwideGrossG_V1.PNG).

![Top 10 movies by average W G bar](https://github.com/apelicier/Phase-2-Project/blob/main/Images/WorlwideGrossG_V1.PNG)

#### Scatter Plot: [Worldwide Gross vs. Average Rating(.PNG)](AverageRating_V2.PNG).

![Average rating scatter](https://github.com/apelicier/Phase-2-Project/blob/main/Images/AverageRating_V2.PNG)

#### Scatter Plot: [Worldwide Gross vs. Number of Votes(.PNG)](NumberOfVotes_V3.PNG).

![Number of votes scatter](https://github.com/apelicier/Phase-2-Project/blob/main/Images/NumberOfVotes_V3.PNG)

#### Heatmap: [Correlation between Average Rating, Number of Votes, and Total Gross(.PNG)](movie1.PNG).

![Correlation heatmap](https://github.com/apelicier/Phase-2-Project/blob/main/Images/movie1.PNG)


## Deliverables
Jupyter Notebook: [Final (.ipynb)](Final.ipynb) (and its PDF export).

Jupyter Notebook_pdf: [notebook (.pdf)](notebook.pdf) Pdf notebook

Non-technical Presentation: [presentation (.pdf)](presentation.pdf) (in pdf format).

GitHub Repository: [This repository itself:](https://github.com/apelicier/Phase-2-Project)

GitHub Repository_pdf: [github (.pdf)](github.pdf)

## Next Steps for the Studio

- Conduct deeper market research within identified top genres.
- Develop concepts that prioritize broad audience appeal and potential for high engagement.
- Strategize talent acquisition and marketing efforts to align with these findings.


##### Contact
[PELICIER Antonine]

[antoninepelicier10@gmail.com)]
