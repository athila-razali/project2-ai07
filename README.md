# Productivity Prediction of Garment Employees
## Summary
**Aim** : To create a model that can predict employees' productivity.     
**Target variable** : actual_productivity = The actual % of productivity that was delivered by the workers. It ranges from 0-1.      
**Data Source** : [UCI: Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Productivity+Prediction+of+Garment+Employees#)
## Methodology
### 1. Data Pipeline
Data is loaded and preprocessed. Taking accounts the unnecessary columns, categorical attributes and missing values. 
With regression approach, the features and labels are identified. The cleaned dataset is split into train and test set with ratio of 80:20.
Data normalization has been made using StandardScaler() module from scikit-learn library.
### 2. Model Pipeline
As data is ready to being trained, the regression problem is addressed using a feedforward neural network model with 3 hidden layers. 
The model has a rather straightforward structure. The model's structure is depicted in the figure below:     
          
![Untitled Diagram drawio](https://user-images.githubusercontent.com/91872382/181933922-d9980ae3-10b4-4b66-bb2a-9acee40eb6a9.png)
           
The model is trained with a batch size of 32 and for 30 epochs.        
The results of the training process are shown in the graph visualized by Matplotlib below:      
          
<img width="289" alt="image" src="https://user-images.githubusercontent.com/91872382/181934004-ee6c2ab6-f5b6-4072-b555-390487c6e4fc.png"> <img width="286" alt="image" src="https://user-images.githubusercontent.com/91872382/181934033-2947530b-5065-4be4-b530-de8fb575f023.png">
            
## Results
The model has been evaluated. The Mean Absolute Error (MAE) is the performance metrics for Regression model.        
The MAE for the actual and predicted values is 0.0994, which means the average difference is lower and a good-fit model.       
A model with good fit should produce a straight line pattern of y=x as the line of best fit in the prediction vs label graph as shown in the figure below:       
<img width="278" alt="image" src="https://user-images.githubusercontent.com/91872382/181934406-8294d513-a9d9-497e-b8e3-7d24633ac8c7.png">
       
### Credits
**Instructor : Kong Kah Chun**       
**Selangor Human Resource Development Center**
