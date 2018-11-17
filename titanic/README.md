# Titanic Dataset.

First of all I haven't considered [ 'Name', 'Cabin', 'Embarked', 'Ticket' , 'Fare' ] into consideration as my features , because I did not felt that , these values as features would do any 
good.

I mean , what impact could a name possibly have on their survivability.

Then I splitted the dataset into training and testing data , and then scaled it , because difference between Age variable and other features was pretty high as you can see in 
the dataset. Now , why I have scaled the features to same scale is because , most of the machine learning models are based on eucladian distance , and thus would not perform 
well on unscaled data , as the data would be skewed heavily towards high value data points ( Age feature in this case ).

After splitting and scaling , I applied 4 different models to test different model's accuracies, which are LogisticRegression model, Knn model, naive_bayes classifier model 
and random_forest model. After applying all the models , I found that the LogisticRegression model outperformed all other models , by maintaing an accuracy of 81%, while other 
models made an accuracy of 77%, 77% and 76% repectively.

After that I just did the same with test data, dropped the unnecessary columns , scaled the columns and then finally predicted the survivability of the passenger on titanic.
