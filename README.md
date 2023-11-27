### Project 1 - Group 1 

## Group 1 – Nida Ballinger-Chaudhary, Eoghan Alton, Ammarah Ahmad, Nana Mensah, Safa Ali

# Project Title: "Evolving Landscapes of Television: An Analytical Dive into TV Show Trends on Netflix"

### Objective:
This project aims to conduct a comprehensive analysis of TV shows available on Netflix, focusing on their evolution over time, the impact of the pandemic on genre popularity, regional production trends, and the relationship between IMDb scores, votes, and genres. The analysis will leverage a primary dataset from Kaggle along with supplementary data from the OMDB API. By examining various aspects such as maturity ratings, genre popularity, production trends, and viewer ratings, the study aims to offer valuable insights for content creators, media strategists, and streaming service analysts.

### Data Sources:
- Primary Dataset: Netflix Movies and Shows dataset from Kaggle, focusing on TV shows (approx. 2500 data points) - https://www.kaggle.com/datasets/maso0dahmed/netflix-movies-and-shows/data
- Secondary Data: Supplemental information from the OMDB API, providing additional details like ratings, languages, and production countries.

### Key Questions:
#### 1. Maturity Rating Evolution:
##### Team Member Responsible - Ammarah
- How do different age certifications (like TV-MA, TV-14) perform in terms of quantity and popularity?
- Does this reflect any broader market trends or shifts in audience demographics?

#### 2. Pandemic and Reality TV Popularity:
##### Team Member Responsible - Safa
- Was there a significant rise in the popularity of reality TV shows during the pandemic, and has this increase been sustained post-pandemic?
- How do scripted TV shows perform in comparison to non-scripted ones in terms of IMDb scores, viewer engagement, and production rates?

#### 3. Genre Production Patterns:
##### Team Member Responsible - Nana
- What can be inferred about Netflix's content strategy based on the genres and types of shows produced?
- How has the diversity of production regions and languages changed over time on Netflix?
- How does Netflix's content portfolio compare with its initial years versus the more recent years?

#### 4. IMDb Score, Votes, and Genre Relationship:
##### Team Member Responsible - Eoghan
- Are certain genres consistently receiving higher ratings and votes?
- Are older shows maintaining popularity, or is there a trend towards newer releases?
- What factors contribute to higher viewer engagement and popularity for TV shows on Netflix? (Consider aspects like genre, production country, language, and runtime.)

### Proposed Methodology:
#### 1. Data Collection and Cleaning:
##### Team Member Responsible - Nida 
- Collect data from the Kaggle dataset and supplement it with additional information from the OMDB API.
- Clean and pre-process the data, ensuring consistency and usability for analysis.

#### 2. Individual Analysis Focus:
 - Each team member will focus on one specific question, conducting in-depth analysis and visualization.
 - Utilize statistical methods and data visualization techniques to extract insights.

#### 3. Data Visualization and Interpretation:
 - Employ tools like Python (Pandas for data manipulation and Matplotlib for visualization) to create insightful charts and graphs.

#### 4. Documentation and Presentation:
##### Team Member Responsible - Nida 
 - Maintaining documentation in a README file, and preparing the presentation slide deck.
 - Also provide support as needed to other team members.


### Overview of Data Collection, Cleanup, and Exploration Process
The process of data collection, cleanup, and exploration was meticulously carried out to ensure that the resulting dataset is both comprehensive and relevant for detailed analysis. The integration of external API data from OMDB significantly enhanced the dataset's utility, making it a robust resource for exploring trends in Netflix's TV show offerings. The prepared dataset, now saved as netflix_shows.csv, is well-positioned to provide insightful answers to the research questions posed in the project.
#### Data Source and Selection
##### Primary Source: 
The initial dataset was sourced from Kaggle, specifically tailored to contain comprehensive information about movies and shows available on Netflix. This dataset was chosen due to its richness in details about each title, such as release year, age certification, runtime, genres, production countries, and IMDb ratings. The focus on Netflix content makes it a valuable resource for understanding current trends in the streaming entertainment industry.
##### API Integration: 
To enhance the dataset, the OMDB API was utilized. This API provided additional details for each show, particularly language information, which was not available in the original dataset. The OMDB API was selected for its extensive database and ease of access, allowing for detailed cross-referencing using IMDb IDs.

#### Collection and Cleanup Process
##### Data Importation and Filtering:
The Kaggle dataset was first imported into a Pandas DataFrame.
The dataset was filtered to focus solely on TV shows (type 'SHOW'), aligning with the project's focus on serialized content.

##### API Data Integration:
Using the OMDB API, language information for each show was retrieved based on their IMDb IDs.
This data was added to the DataFrame, providing a more comprehensive view of each show.

##### Data Cleanup:
The genres column, initially containing string representations of lists, was transformed into actual lists for easier analysis - and the use of the explode function later on.
Rows without IMDb IDs were dropped to ensure completeness and reliability of the data.
The DataFrame was saved as netflix_shows.csv for subsequent analysis, ensuring a clean and enhanced dataset.

#### Exploration Process
##### Preliminary Exploration:
An initial exploration of the dataset was conducted to understand its structure, the types of data available, and the quality of the data.
Key columns like 'genres', 'release_year', 'imdb_score', and 'production_countries' were examined for patterns and distributions.

### Data Analysis, Visualisation and Interpretation

#### 1. Maturity Rating Evolution:
##### Team Member Responsible - Ammarah
- How do different age certifications (like TV-MA, TV-14) perform in terms of quantity and popularity?
- Does this reflect any broader market trends or shifts in audience demographics?

#### 2. Pandemic and Reality TV Popularity:
##### Team Member Responsible - Safa
- Was there a significant rise in the popularity of reality TV shows during the pandemic, and has this increase been sustained post-pandemic?
- How do scripted TV shows perform in comparison to non-scripted ones in terms of IMDb scores, viewer engagement, and production rates?

#### 3. Genre Production Patterns:
##### Team Member Responsible - Nana
- What can be inferred about Netflix's content strategy based on the genres and types of shows produced?
- How has the diversity of production regions and languages changed over time on Netflix?
- How does Netflix's content portfolio compare with its initial years versus the more recent years?

#### 4. IMDb Score, Votes, and Genre Relationship:
##### Team Member Responsible - Eoghan
- Are certain genres consistently receiving higher ratings and votes?
- Are older shows maintaining popularity, or is there a trend towards newer releases?
- What factors contribute to higher viewer engagement and popularity for TV shows on Netflix? (Consider aspects like genre, production country, language, and runtime.)
