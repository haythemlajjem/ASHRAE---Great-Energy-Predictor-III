# ASHRAE---Great-Energy-Predictor-III

This project has been made for the kaggle competition ASHRAE---Great-Energy-Predictor-III : Prediction of  Building consumption energy with a deep learning model

The Notebook has 6 parts :
   
    1/ Importing the nedded packages such as : keras, sklearn, pandas, numpy, matplotlib
    2/ Uploaing train.csv  and cleaning it : dividing timestamp in 3 clumns 
    3/ Uploading building_metadata.csv and cleaning it : deleting year_built and floor_count columns , 
    Label encoding for primary_use column , log normalization for square feet 
    4/ Uploading weather_train.csv and cleaning it : deleting air_temperature coliumn ,log normalisation for 
    dew_temperature and wind_speed columns, filling missed values by the previous one 
    5/ Merging data 
    6/ Building a DL Model with this summary :
     Layer (type)                 Output Shape              Param #   
      =================================================================
     dense_5 (Dense)              (None, 200)               2400      
      _________________________________________________________________
     dropout_4 (Dropout)          (None, 200)               0         
     _________________________________________________________________
     batch_normalization_4 (Batch (None, 200)               800       
     _________________________________________________________________
     dense_6 (Dense)              (None, 100)               20100     
     _________________________________________________________________
     dropout_5 (Dropout)          (None, 100)               0         
     _________________________________________________________________
     batch_normalization_5 (Batch (None, 100)               400       
     _________________________________________________________________
     dense_7 (Dense)              (None, 50)                5050      
     _________________________________________________________________
     dropout_6 (Dropout)          (None, 50)                0         
     _________________________________________________________________
     batch_normalization_6 (Batch (None, 50)                200       
     _________________________________________________________________
     dense_8 (Dense)              (None, 1)                 51        
     =================================================================
     Total params: 29,001
     Trainable params: 28,301
     Non-trainable params: 700
     _________________________________________________________________
     
       
You can find data on this link  "https://www.kaggle.com/c/ashrae-energy-prediction"
