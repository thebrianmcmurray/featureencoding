# Feature Encoding Analysis

This is the analysis that I performed as part of my final project for my Master's degree in Data Analytics. The project was to compare different methods of encoding categorical features with high cardinality. For a full explanation of the project, please refer to the Feature Encoding Analysis.pdf file.

These encoding methods will be tested: 
- Multiple Correspondence Analysis (MCA)
- K-Modes clustering
- James Stein target encoding
- M-Measure encoding
- CatBoost encoding

## Files
- **Feature Encoding Analysis.pdf**: The paper I wrote for this analysis. It was written in LaTeX.
- **Housing Market Analysis.ipynb**: The Python notebook used to perform the analysis and generate various charts and tables used in the paper.
- **Real Estate Scraper.ipynb**: The Python notebook used to scape a local real estate website to build the dataset. The original website has changed its terms of service since the analysis was initially performed, so I have removed any references to it out of respect to their updated terms.
- **Results.csv**: The performance results for each encoding method across each model that was tested.
- **housingData.csv**: The resulting dataset created by the Real Estate Scraper notebook.

## Results

For the analysis, six different feature encoding methods were compared. To compare their effectiveness, the dataset was encoded using each method, and then four different predictive models were trained and evaluated 20 times for each method. The clustered box plot below shows the adjusted R2 scores for each encoding method with each predictive model type.
![Results](https://github.com/thebrianmcmurray/featureencoding/blob/main/meanrsquare.png?raw=true)
