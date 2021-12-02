# Hospital-Playlist

### Data_Cleaning_Master_Data.ipynb: 
The code for cleaning and processing the master data in preparation for data visualization and modelling.

### Visualization_and_Modelling.ipynb: 
Contains the code for preliminary data visualization and modelling. 
For modelling, the code consists of preprocessing (with PCA(), MinMaxScaler(), and StandardScaler()) and modelling with Logistic Regression, kNN, Regression Tree, Support Vector Classification, and Support Vector Regression

### Preprocessing and Modeling without Genres.ipynb:
Contains the code for preliminary data visualization and modelling where binary genre information has not yet been integrated into the dataset. 
For modelling,the code consists of preprocessing (with PCA(), MinMaxScaler(), and StandardScaler()) and modelling with Decision Trees, Ensemble Classifier, Ridge Regression and Lasso Regression to predict trauma, total health and specific mental health indicators.

### Data Collection, Cleaning and Spotipy.ipynb:
Contains the code for song data collection, before merging with preliminary song data and cleaning. The combined information was then used to extract information from the Spotify Web API using Spotipy. 

### Preprocessing and Modeling with Genres.ipynb:
Contains the code for secondary data visualization and modelling where binary genre information has been integrated into the dataset. 
For modelling,the code consists of preprocessing (with PCA(), MinMaxScaler(), and StandardScaler()) and modelling with Decision Trees, Ensemble Classifier, Ridge Regression and Lasso Regression to predict trauma, total health and specific mental health indicators.

### model_eval.ipynb: 
Contains code to clean data in order to visualize the models for each target. Finds the best preprocessing step for classification and regression model for each target. 
