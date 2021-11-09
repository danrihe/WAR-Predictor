# WAR-Predictor

## Repository Contents
- **FanGraphs-Pitching-Advanced.csv:** Dataset used to create working dataset. Contains advanced statistics on eligible pitchers.
- **FanGraphs-Pitching-Standard.csv:** Dataset used to create working dataset. Contains basic statistics on eligible pitchers.
- **FanGraphs-Pitching-Value.csv:** Dataset used to create working dataset. Contains statistics to quantify a pitcher's value.
- **master-dataset.ipynb:** Python script used to create the working dataset by joining the three datasets listed above.
- **pitching-masterdataset.csv:** Working dataset created by the master-dataset.py script.
- **WAR-predictor.ipynb:** Python script used to construct multiple linear regression model and random forest regression model.

## Tentative Project Stages
1. **Dataset Creation:** Create a masterdataset using the three subsets from FanGraphs. This dataset is created by joining the three original datasets on playerid, Season, Name, and Team.
2. **Data Preprocessing:** Involves removing the % sign from fields that contain them and ensuring that data is in a useable format.
3. **Splitting Training & Testing Datasets:** Split the working dataset into a training dataset and testing dataset. The working dataset is split as follows: 75% training set, 25% testing set.
4. **Creating Multiple Linear Regression Model:** Create a multiple linear regression model using the training set and use it to predict the WAR values for the testing set.
5. **Creating Random Forest Regression Model:** Create a random forest regression model using the training set and use it to predict the WAR values for the testing set.
6. **Analyze Results:** Compare the predicted values for both models and compare against the actual WAR (expected values). Pull summary statistics for both models to determine efficiency, accuracy, and stability.