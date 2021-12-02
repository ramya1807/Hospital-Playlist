# Hospital-Playlist

### Data_Cleaning_Master_Data.ipynb: 
The code for cleaning and processing the master data in preparation for data visualization and modelling.

### Preliminary Visualization.ipynb:
Contains the code for preliminary data visualization and classification models. For modelling, no preprocessing was used and models were Decision Trees and Ensemble Classifier.

Visualizations include
* Distribution of hours spent listening to music mapped to health variables
* Trauma mapped to each song variable (energy to popularity).
* Total health mapped to each song variable (energy to popularity).
* Total health mapped to each song variable (energy to popularity) and grouped by trauma.

Modelled relationships include
* map song variables to amount of music
* map song variables to total health
* map song variables to trauma
* predict trauma with non-health variables (excludes health indicators, total_health, health_categorical, trauma)
* predict total health with non-health variables
* predict specific health variable with non-health variables

### Visualization_and_Modelling.ipynb: 
Contains the code for preliminary data visualization and modelling. 

The preprocessing methods used include
* MinMaxScaler()
* StandardScaler()
* PCA()

The models used include 
* Logistic Regression
* kNN
* Regression Tree
* Support Vector Classification
* Support Vector Regression

### Preprocessing, Preliminary Modeling and Spotipy.ipynb:
Contains the code for preliminary data visualization for individual variables and in relation to other variables, and modelling where binary genre information has not yet been integrated into the dataset. Also contains the code for generating the Spotify id and preview url for 30s Spotify previews of all tracks using Spotipy. The urllib package was then used to retrieve the mp3 files of all the songs with preview urls present.
For modelling,the code consists of preprocessing (with PCA(), MinMaxScaler(), and StandardScaler()) and modelling with Decision Trees, Ensemble Classifier, Ridge Regression and Lasso Regression to predict trauma, total health and specific mental health indicators.

### Data Collection, Cleaning and Spotipy.ipynb:
Contains the code for song data collection, before merging with preliminary song data and cleaning. The combined information was then used to extract information from the Spotify Web API using Spotipy. 

### Preprocessing and Modeling with Genres.ipynb:
Contains the code for secondary data visualization and modelling where binary genre information has been integrated into the dataset. 
For modelling,the code consists of preprocessing (with PCA(), MinMaxScaler(), and StandardScaler()) and modelling with Decision Trees, Ensemble Classifier, Ridge Regression and Lasso Regression to predict trauma, total health and specific mental health indicators.

### Mel_Spectrogram_and_CNN.ipynb
Contains the code for tertiary data modelling where mp3 files were converted to wav files using pydub, that were then used to generate Mel Spectrogams using Librosa. The spectrograms were then sorted based on their classifications before separated using splitfolders into their training and validation sets (70%-30%). The images were then used to perform CNN using Resnet50 to predict trauma and specific mental health indicators.

### model_eval.ipynb: 
Contains code to clean data in order to visualize the models for each target. Finds the best preprocessing step for classification and regression model for each target. 
