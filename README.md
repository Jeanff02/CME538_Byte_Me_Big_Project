# U.S. University Recommendation Tool
Every year, millions of high school graduates face challenges navigating the complex process of choosing the right university. Although plenty of data is available for each institution, it can be overwhelming for students to look through and match with their personal criteria. Traditional university rankings often overlook student sentiment, providing little insight into how current students perceive their own universities.

This tool is designed to offer students personalized recommendations for U.S. universities and colleges that align with their individual preferences. It uses a comprehensive dataset featuring the top 50 universities in the U.S. by academic reputation, based on the QS World University Rankings (https://www.topuniversities.com/world-university-rankings).

#### Link to Medium Article:
https://medium.com/@williampark0211/post-secondary-education-c43a206044a9

## Installation Instructions
1. Open your terminal or command prompt.
2. Clone the repository using the following command:
```
git clone https://github.com/Jeanff02/CME538_Byte_Me_Big_Project.git
```
3. Navigate to the directory: `CME538_Byte_Me_Big_Project`

## How to Use the Tool

1. Navigate to the `Recommendation Model` folder.
2. Open the file `recommendation_model.ipynb`.
3. Run the code in the notebook. You will be prompted to assign an importance value to each of the following metrics:
- Tuition: Annual cost of attending the university.
- Number of Students: Size of the student body.
- Retention Rate: Percentage of first-year students who continue their studies at the same university.
- Diversity Score: Measure of the international diversity of the student population.
- Research Score: Research reputation and output.
- Employer Reputation: How employers perceive graduates from the university.
- Campus Size: Physical size of the campus.
- Safety Score: Security of the campus and the surrounding area.
- Social Score: Social life, including clubs, events, and campus culture.
- Sentiment: Feedback and opinions from current and former students about their university experience.
4. The tool will generate a list of recommended universities based on your input. The recommendations will be saved as `recommended_universities.csv`.

For more insights, you can scroll through the notebook for the following:
- A 3D plot displaying five clusters of universities based on the three highest importance metrics.
- The probabilities of selecting each cluster.
- Outliers that were excluded from the model.

## Dataset Information
Datasets are located in the `Data Collection` folder.
To recreate the data:
- Run the .ipynb files in the respective subfolders to generate the .csv files.
- The `combined_data.ipynb` file in the `Data Merging + Cleaning` folder merges and cleans the datasets to produce the `merged_datasets.csv` file, which is used as the input for the model.

## Exploratory Data Analysis
Data visualizations can be found in the `Exploratory Data Analysis` folder. These visualizations show interesting patterns and informed the selection of inputs for the recommendation model.

## Data Sources
- LawnStarter Campus Size (https://www.lawnstarter.com/blog/college-rankings/biggest-college-campuses-in-us/)
- NTU Research Rankings (https://nturanking.csti.tw/ranking/OverallRanking/)
- QS World University Rankings (https://www.topuniversities.com/world-university-rankings)
- RateMyProfessors (https://www.ratemyprofessors.com/)
- College Scorecard (https://collegescorecard.ed.gov/)

## Attribution Table

| **Name**   | **Contributions**                                           |
|------------|-------------------------------------------------------------|
| Daniel     | College Scorecard, QS Ranking Data, Clustering Data         |
| Mohamed    | NTU Scraping, Classification & Recommendation Model         |
| William    | MeteoStats Data, Exploratory Data Analyses (EDAs)           |
| Jean       | Rate My Professor Data, User Input                          |