# AI-Credit-Risk

The use of AI and its applications in the many industries exceeds what we may believe. One of which is the financial industricies and its many intricacies surrounding risks such as credit risk. By using various metrics such as income, payment time, schedule, and other important facotrs, financial companies can determine the risk an individual poses when they are requesting some sort of loan. In this module, we will use different models to determine which is the most effective in determining credit risk.

## Results


4 similar resampling techniques were used from the imblearn library: 2 forms of Oversampling, 1 Undersampling and 1 Combination sampling (if you want more information on these, visit [this link](https://machinelearningmastery.com/random-oversampling-and-undersampling-for-imbalanced-classification/). In summary, due to large differences in populations of our data sets, we will be randomly duplicating/deleting examples in within the respective class to create a more even distrubition for better analysis. However, within these algoriths, there are multitudes of libraries that exists but in this module, we will not go over the differences, only the results. 

Aside from resmapling we also used ensemble learners which use multiple algorithms. In this module we use random forest and easy ensemble.

The general code is relatively straight forward and consistent. The data was split into our training and testing data and strings were converted to numbers to provide a more "computer friendly" information. From there, we used the train_test_split function  and then instantiated the algorithms we plan to use and then finally, fit the model and summarize the data.

The summaries are provided below in the order of Accuracy, Classification report, and imbalanced matrix

### Naive Random Oversample

![combination acc](https://user-images.githubusercontent.com/100324759/177014403-c8288905-ef07-4379-9f8f-45004df975dc.PNG)

![comb report](https://user-images.githubusercontent.com/100324759/177014402-1e5a978f-8ffe-4ba5-a577-7b04d4e854b2.PNG)

![comb matrix](https://user-images.githubusercontent.com/100324759/177014401-ab70fd66-7ca2-4bb6-9150-ddc46de9fa3f.PNG)


### SMOTE Over sample

![smote over acc](https://user-images.githubusercontent.com/100324759/177014412-37e6049a-08c2-4cba-be9e-ec24130faf9b.PNG)

![over report](https://user-images.githubusercontent.com/100324759/177014411-8a3c4527-424d-4411-aa20-e1bd9062872d.PNG)

![Smote over matrix](https://user-images.githubusercontent.com/100324759/177014413-2a8abb1a-4279-4a25-a249-58b321c7982e.PNG)


### Random Undersample


![under acc](https://user-images.githubusercontent.com/100324759/177014415-f60cbb87-cfd6-447a-9f11-5bf152df6cf2.PNG)

![under report](https://user-images.githubusercontent.com/100324759/177014417-8dc7605d-904c-4b5e-8e06-87a33bacc7af.PNG)

![under matrix](https://user-images.githubusercontent.com/100324759/177014416-31e8a535-8265-4ef0-bad3-29f183875d0a.PNG)


### Combination 

![combination acc](https://user-images.githubusercontent.com/100324759/177014422-8abe60ea-25bb-4d64-bb61-4926a8916e94.PNG)

![comb report](https://user-images.githubusercontent.com/100324759/177014421-ae86ca48-647f-49e5-803f-5c63f9515e42.PNG)

![comb matrix](https://user-images.githubusercontent.com/100324759/177014420-917300b4-d3cd-4b90-bee9-b0158bbf821d.PNG)



### Random Forest Ensemble

![forest acc](https://user-images.githubusercontent.com/100324759/177014431-dc6ec560-8f56-400b-8a44-1db51262afba.PNG)

![forest report](https://user-images.githubusercontent.com/100324759/177014430-f05ec677-d964-46e6-b639-73b226c0f84b.PNG)

![forest matrix](https://user-images.githubusercontent.com/100324759/177014428-a476b4ad-72fa-4259-b8b2-513fa36c438f.PNG)




### Easy Ensemble

![easy ensemble acc](https://user-images.githubusercontent.com/100324759/177014437-25da675a-7236-4089-ac72-11b5ba90d902.PNG)

![easy report](https://user-images.githubusercontent.com/100324759/177014439-ae5af130-cc3b-46da-b012-3e488368b949.PNG)

![easy matrix](https://user-images.githubusercontent.com/100324759/177014438-21e0e8ee-4786-4d54-93ab-89661f247220.PNG)



## Summary

Although each method provided us with a prediction, not each had the desired results. From the 6 machine learning models, the ensemble methods were the most consistent in all three sections of measure: accuracy, precision and recall. The sampling techniques had accuracy scores of approximately 60% which is quite low, furthermore, the poor precision and recall (except for combination with 99% precision) provide far too inconsistent results. The ensemble methods are all 70% in each of the metrics and provide a level of consistency that is great for banks wanting to assess risk. Of the 6 models, considering they all require the same effort, easy ensemble is the best option to use. 
