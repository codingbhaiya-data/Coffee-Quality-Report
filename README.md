# Coffee-Quality-Report
## Introduction 
The Coffee Quality Institute (CQI) is a non-profit organization that works to improve the quality and value of coffee worldwide. It was founded in 1996 and has its headquarters in California, USA.
CQI's mission is to promote coffee quality through a range of activities that include research, training, and certification programs. The organization works with coffee growers, processors, roasters, and other stakeholders to improve coffee quality standards, promote sustainability, and support the development of the specialty coffee industry.

## Objective 
The objective of this project is to explore the factors that influence coffee quality, including sensory attributes, processing methods, and regional origins.
he analysis aims to provide insights into the relationships between these factors and overall coffee quality scores, identify trends in defect occurrences, and understand how different variables interact to affect the total cup points.

## Dataset 
The data includes a range of information on coffee production, processing, and sensory evaluation. It also contains data on coffee genetics, soil types, and other factors that can affect coffee quality.

Sensory evaluations (coffee quality scores)
- Aroma: Refers to the scent or fragrance of the coffee.
- Flavor: The flavor of coffee is evaluated based on the taste, including any sweetness, bitterness, acidity, and other flavor notes.
- Aftertaste: Refers to the lingering taste that remains in the mouth after swallowing the coffee.
- Acidity: Acidity in coffee refers to the brightness or liveliness of the taste.
- Body: The body of coffee refers to the thickness or viscosity of the coffee in the mouth.
- Balance: Balance refers to how well the different flavor components of the coffee work together.
- Uniformity: Uniformity refers to the consistency of the coffee from cup to cup.
- Clean Cup: A clean cup refers to a coffee that is free of any off-flavors or defects, such as sourness, mustiness, or staleness.
- Sweetness: It can be described as caramel-like, fruity, or floral, and is a desirable quality in coffee.
     ### Defects:
Defects are undesirable qualities that can occur in coffee beans during processing or storage. Defects can be categorized into two categories: Category One and Category Two defects.
- Category One defects are primary defects that can be perceived through visual inspection of the coffee beans. These defects include Black beans, sour beans, insect-damaged beans, fungus-damaged beans, etc.
- Category Two defects are secondary defects that are more subtle and can only be detected through tasting. These defects include Over-fermentation, staleness, rancidness, chemical taste, etc.

## Steps Undertaken to Create Dashboard 
1. *Loading Data:* The datasets were imported into Power BI from various sources, including CSV files and Excel spreadsheets.
2. *Transforming Data:* Using Power Query Editor, data was transformed to ensure consistency and accuracy. This included:
      - Renaming columns for clarity
      - Converting data types
      - Merging and appending tables as necessary
3. *Cleaning Data:* Data cleaning involved handling missing values, removing duplicates, and filtering out irrelevant data.
4. *Creating Relationships:* Relationships between tables were established to ensure proper data connectivity and analysis. For instance, linking sensory scores with their corresponding coffee samples and processing methods.
5. *Adding Calculated Columns and Measures:* DAX (Data Analysis Expressions) formulas were used to create calculated columns and measures essential for analysis.

## Dashboard Requirements
The dashboard includes various visualizations to provide a comprehensive overview of the data:
- Score Distribution: Bar charts and histograms showing the distribution of sensory scores.
- Regional Analysis: Maps and charts highlighting coffee quality variations across different regions.
- Processing Methods: Pie charts and bar graphs depicting the impact of processing methods on coffee quality.
- Defect Analysis: Scatter plots and line charts illustrating trends in defect occurrences.



## DAX Formulas Used 
Some of the key DAX formulas used in the project include:
- Total Score: Total Score = SUM(SensoryScores[Score])
- Average Score: Average Score = AVERAGE(SensoryScores[Score])
- Defect Percentage: Defect Percentage = DIVIDE(COUNT(Defects[DefectID]), COUNT(CoffeeSamples[SampleID]), 0)

## Questions and Analysis : 
1. What are the key factors contributing to high coffee quality scores?
-> Analyzed sensory attributes and identified which attributes most significantly influence the total cup points.
2. How do processing methods affect coffee quality?
-> Compared the average quality scores across different processing methods.
3. Are there any regional trends in coffee quality?
-> Mapped out the regions to see which areas produce the highest quality coffee.
5. What trends exist in defect occurrences, and how do they impact quality?
-> Identified patterns in defect occurrences and their correlation with quality scores.

## Conclusion 
he analysis revealed that certain sensory attributes, such as flavor and aroma, are strong indicators of high coffee quality. Processing methods also play a significant role, with washed and natural methods generally yielding higher quality scores. Additionally, specific regions consistently produce superior coffee, highlighting the importance of origin in coffee quality. The findings from this project can help coffee producers and marketers focus on the key areas that enhance coffee quality, ultimately leading to better products and customer satisfaction.

