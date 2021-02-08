# Twitter Sentiment Analysis


# Overview:
## For this project, I set out to create a model that would have the greatest accuracy on rating the sentiment of a dataset full of unedited tweets. While some challenges arose during the process, I ultimately recieved an accuracy score I was happy with by utilizing both neural network and random forest models.


# Preprocessing:



<img src="Pictures/Uncleaned_Text">



## Preprocessing the data was the most time consuming part of project. Since I was working with tweets, I had to make sure to get rid of all the unnecessary objects and characters to be left with the most basic version of the tweet possible while still keeping the most important words. After the cleaning process, I was able to make each tweet look something like this:


<img src="Pictures/Cleaned_Text">


# Most common words throughout the dataset:



<img src="Pictures/word_bank">



# I ultimately had to upsample the data because there were so few negative and positive classifiers as opposed to neutral ones. Below is th neural network that ultimately gave me my highest accuracy score, as well as a graph showing the difference in loss and accuracy between the training and validation data.



<img src="Pictures/nn_code">
<img src="Pictures/graphs">
<img src="Pictures/accuracy">



# While the loss and accuracy graphs for the trainign and validation data are not entirely the same, precautions would have needed to be taken if the lines in either of the graphs were diverging from eachother.


# Overall, the neural network shown above was able to send back a model with the highest accuracy. As always with classification problems, I thought looking at the confusion matrix might be very useful in terms of what to possibly consider for future research.

<img src="Pictures/matrix">


# As we can see, the negative class received the most incorrect predictions, partly due to the fact that the dataset was lacking negative sentiments. This then led to the model not being properly trained on classifying negative tweets compared to classes with more data.
