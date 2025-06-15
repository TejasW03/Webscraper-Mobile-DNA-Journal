# Webscraper-Mobile-DNA-Journal
Web scraping and data visualization of academic articles published in the Mobile DNA journal.

This project automates the extraction, cleaning, and analysis of article metadata from the *Mobile DNA* journal using R. It was developed as part of the **DS636 - Data Science** course at **New Jersey Institute of Technology (NJIT)**.

## Objective

The goal of this project is to:
- Programmatically scrape academic article data from the *Mobile DNA* journal (BioMed Central)
- Extract key fields such as title, abstract, authors, keywords, publication date, and corresponding author info
- Analyze publication trends and identify patterns in authorship and keyword usage
- Visualize the data using R libraries like `ggplot2` and `viridis`

---

## What the Script Does

1. **Scrapes journal data** from the selected volume/year of the Mobile DNA journal
2. **Extracts metadata** for each article:
   - Title
   - Author list
   - Abstract
   - Keywords
   - Corresponding author & email
   - Publication date
3. **Cleans and preprocesses** the extracted data
4. **Generates visualizations** including:
   - Monthly publication trends
   - Top 10 corresponding authors
   - Top 10 most-used keywords
5. **Exports final results** as a CSV (`final_scraped_data.csv`)

---

## Technologies & Libraries Used

This project was implemented in **R**, with the following packages:

| Library       | Purpose                          |
|---------------|----------------------------------|
| `rvest`       | Web scraping                     |
| `xml2`        | HTML parsing                     |
| `httr`        | HTTP requests                    |
| `dplyr`       | Data manipulation                |
| `stringr`     | String handling                  |
| `tidyr`       | Data reshaping                   |
| `ggplot2`     | Visualization                    |
| `viridis`     | Visualization color palettes     |

---

## How to Use

Clone this repository
   ```bash
   git clone https://github.com/<your-username>/webscraping-mobile-dna.git
   ```
Open the R script

Run the script
You will be prompted to enter a year (between 2010 and 2024). The script calculates the volume and proceeds to scrape all articles in that volume.

## Visualizations

### Publication Trends Over Time
Shows the number of articles published each month over time.
![Publication Trends](https://github.com/TejasW03/Webscraper-Mobile-DNA-Journal/blob/main/images/image1.PNG?raw=true)

### Top 10 Corresponding Authors
Most prolific authors based on article count.
![Top Authors](https://github.com/TejasW03/Webscraper-Mobile-DNA-Journal/blob/main/images/image2.PNG?raw=true)

### Top 10 Keywords
Most common keywords used in Mobile DNA publications.
![Top Keywords](https://github.com/TejasW03/Webscraper-Mobile-DNA-Journal/blob/main/images/image3.PNG?raw=true)
