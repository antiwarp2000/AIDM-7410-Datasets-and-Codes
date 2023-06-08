# AIDM-7410 Datasets-and-Codes

# Project Introduction

This repository was created in the Semester 2 of 2022-2023. It stores the group project datasets&codes of the course AIDM-7410 Computational Journalism @ Hong Kong Baptist University, School of Communication (HKBU). This group project was created by <b>JIANG Zhuohao, YU Minghao, and HE Yuchen</b>.

We have utilized AI techniques/models and visualization components to create a data-driven news work focused on the World Press Photo (WPP) contest.

Specifically, we have collected and analyzed 2,880 entries and over 12,800 photos from all WPP awards since 1955, along with examination on descriptions of these award-winning photos and information about the photographers published on the official WPP website. 

![Image Description](https://raw.githubusercontent.com/antiwarp2000/AIDM-7410-PAGE/main/illustrations/0001.png)


Our goal was to identify trends and characteristics of WPP awards both externally and internally, strive to demonstrate the overall criteria and taste of WPP awards (and their trends), and ultimately tend to acquire the answer and a guidance for you who are interested: <br><b>WHAT MAKES A PRIZE IN World Press Photo CONTESTS?</b>

<b>The following is the content of web-scraping, AI analysis & visualisation details.</b>

# Directory Structure Description
    ├── ReadMe.md           // help document
    
    ├── output    //  database files that need to be used 

        │   ├── dfimage    // Every photo's information with local storage path by year

    │   ├── dfimageurl    // Every photo's information with image url by year

    │   ├── database_photographer_all.csv   // Every photographer's official information stored in WPP's website combined

    │   ├── dfimageurlall.csv   // Every photo's information with image url combined

    │   ├── dfimageurlall_summerized.csv   // Every photo's information with shorten description

    │   ├── dfimageurlall_summerized_location.csv   // Every photo's information with shorten description and location

    │   ├── timeline   // Awards per country over time

    │   ├── new_df_country(3).csv  // Database for earth model establishment after manual correction of locations
    
    │   ├── photographer   // Top 10,Top 20 photographer 
    
    │   ├── prizegroup  // Distribution of awards for protest-related photos

        │   ├── dfphotographer.csv    // Every works' direct link of presentation page



    
    ├── code           // The core code part, including the basic implementation process of each part
	
    
    │   ├── ScrapeURL.ipynb    // Scrape all stored photos' information and photo url

        │   ├── ImageDownload.ipynb    // Download every photos to local for AI analysis

    │   ├── Summerization.ipynb    // Use pre-trained Flan-T5 model to shorten the description of photo stories

        │   ├── Location-detection.ipynb    // Use UIE base model in cooperation with Spacy and PyCountry library to extract the exact location of each photo where it was taken

    │   ├── Combine picture.ipynb    // Stitch pictures
    
    │   ├── country net.ipynb    // Extraction of the country where the photo was taken, analysis of the photographer's footprint
    
    │   ├── photographer.ipynb    // Recap of awards for all countries

Final integration + computational journalism content presentation:

[What make a Prize? Presentation Webpage](https://antiwarp2000.github.io/AIDM-7410-PAGE/)
