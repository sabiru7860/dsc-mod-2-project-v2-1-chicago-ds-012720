# Intro
My main goal for this project was to see how diffrent features effect hosuing prices.

#Prereqiusistes
I used multiple python libraries for my analysis. For visuals i used matplotlib. i used sklearn and stats model for data preprocessing and also to run my model.

# Models
I decided to make 3 models for my project. For my first model i decided to run a rough baseline model. I have gotten an R squared of 65 percent

For my second model i decided to try to scale my data using a standerd scalar method using sklearn
```
ss = StandardScaler()
column2= modelX2_train.columns
modelX2_train = pd.DataFrame(ss.fit_transform(modelX2_train))
modelX2_train.columns = column2
```
I also decided to compare multiple features to the sqft of living to try and improve my model. For model 2 i got an R squared of 68 percent

For my last model i decided to use the natural log of my coefficents to help my model. This will get my coefficents more normal normally distributed. After testing out my model i got an R squared of 51 percent.


#Conclusion
Overall my model 2 worked the best. Using the standard scalar method and also adding new variables helped my model predict better.