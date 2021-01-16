Diamond Dataset

Table of Content:
1. Introduction and Objective
2. Dataset Description
3. Data Preprocessing and Visualization
4. Modeling Phase
5. Conclusion

1. Introduction and Objective:

      Diamond Dataset is provided with different features. Our main Objective is to predict the price of Diamond against other features.
      
2. Dataset Description:

      The data definition is as follows:

        carat: Weight of the diamond

        cut: Quality of the cut (Fair, Good, Very Good, Premium, Ideal)

        color: Diamond color

        depth: Total depth percentage (it is calculated as: 2 * z / (x + y))

        table: Width of top of the diamond relative to the widest point

        price: Price of a diamond in US dollars (target/dependent variable)

        x: Length of a diamond in mm

        y: Width of a diamond in mm

        z: Depth of a diamond in mm

3. Data Preprocessing and Visualization:

        For all the dataset, Checking null value is very important. In this dataset, there is no null values. Some of the data's are catergorical in nature.
        To perform Linear Regression Model need to encode and for Linear Regression Outlier plays very important role. To avoid outlier affecting model performance,
        Capping was performed. Now the dataset is ready to build the model.
        
 4. Modeling Phase:
        OLS model is built based on input and target column.
        Before proceeding to build model further, 5 assumption like Multicollinearity,Normality,Linearity,Autocorrelation,Homoscadacity is checked for Linear Regression method.
        "table","depth","y","color","cut" are the features statisfying multicollinearity test.
        While testing for Normality, it not statisfied. After transforming the target, model statisfied Normality i.e Data is normally distributed and skewness also reduced.
        While checking for model Linearity it is not statisfied. Tried to transform all the input features. Evenafter transforming input model is not statisfying the Linearity.
        
 5. Conclusion:
        
        So this Diamond Dataset is not suitable to perform Linear Regression Model. In future, this model will be built based on some Non - Linear Algorithms.
