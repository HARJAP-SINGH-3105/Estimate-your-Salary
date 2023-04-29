# Estimate-your-Salary

##                                                    Project Objective

To develop a comprehensive database of estimated salary for various job roles in the industry, including data scientists, software engineers, and others. The objective was achieved by scraping data from websites like Glassdoor and Indeed, converting it into usable form, and performing further analysis. The project will leverage features like company rating, location, type of ownership, and job title to create reliable estimates of salary offered for different roles in the industry.



                                           
##                                                  LEARNING FROM THE PROJECT:
                      
### Data Synthesis - Scrapping 

#### Challenges:
-Do not have to use already synthesised data from kaggle or any other project
-Most of websites lack desired information like ‘Company rating’ or ‘Salary’ etc.
-Even if some features are available then these are marked as ‘Unknown’.

#### Approach:
-Use the ‘Selenium’ library and write code to scrap the data
-Manually put lot of efforts in searching useful page that contain most features
-Use Excel to remove some arbitrary values 

#### Learning:
-During this whole process, learn how actually data is synthesised and prepared for ML project

### Deep dive into Regression

#### Challenges:
-Naive models like simple linear regression are working but can be further reduce the ‘RMSE’ or have a more better model?
-Advanced models like ensemble model, boosting model etc. have large number of hyperparameters, how to choose them?
- How to ensure that our model is not overfitting the data?

#### Approach:
- Implement the more robust models like ‘Random Forest’ and ‘Adaboost’ and compare the results obtained
-Compute and plot errors for both testing and training data to ensure that model do not overfit the data
-Use GridSearchCV, K-Fold and other techniques to tune the hyperparameters of models

#### Learning:
-learn the how to implement , compare and tune the different regression models 

### Missing values

#### Challenges:
-Many features of the scrapped data have high percentage of missing values.
-Know the various techniques of imputing missing value but main problem is how to choose which is the best to apply for given data?

#### Approach:
-Some of the feature has upto 65% of values as NaN, so firstly check its relation with rest of data and then decide whether to drop that feature or not
-if not dropped, following approach is used:
Make the two copied of given dataset and randomly choose 30% (just a random number) those rows of features which does not have null value
Store the indexes of the above chosen rows
Now try to impute the values of whole real-valued feature by the any of the above techniques for just one copy of dataset
Now compute the MSE (mean squared error) of imputed values and orignal dataset values corresponding to the chosen rows in step 2
Method which give the lowest MSE will be selected


Note: Other approach: Checking the performance of model on imputed values of each technique and then decide which technique to apply can also be used 


#### Learning:
-Learn how to deal with missing values and which method to choose
<img width="621" alt="image" src="https://user-images.githubusercontent.com/84041223/235301059-10370800-6c49-4830-880b-3f8db452d4a0.png">
<img width="549" alt="image" src="https://user-images.githubusercontent.com/84041223/235300981-e0752349-eb64-4735-86fa-9601d292373a.png">

<p>
<img width="736" alt="image" src="https://user-images.githubusercontent.com/84041223/235300850-649fd535-b539-49f7-82af-02bd85ef5a27.png">
</p>
<p>
<img width="393" alt="image" src="https://user-images.githubusercontent.com/84041223/235300881-05b28eae-b8cd-4611-998d-61d6454643dc.png">
<img width="394" alt="image" src="https://user-images.githubusercontent.com/84041223/235300892-3abf96df-7740-4932-87fb-824b244aacc2.png"></p>
<p><img width="394" alt="image" src="https://user-images.githubusercontent.com/84041223/235300901-25169653-2bd6-4f79-82be-db78f230bdcc.png">
<img width="396" alt="image" src="https://user-images.githubusercontent.com/84041223/235300912-f36e482e-a068-4f2f-8c69-b1ecc00ac4e8.png"></p>
<p><img width="385" alt="image" src="https://user-images.githubusercontent.com/84041223/235300926-1b1abeaa-51a1-4b7e-83c5-850509146c4d.png"></p>

 






   
