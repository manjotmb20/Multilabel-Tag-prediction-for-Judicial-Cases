# Multilabel-Tag-prediction-for-Judicial-Cases

The model uses the court case statements to extract different tags that might summarize the judicial case statement.
Being a multi label classification task, in order to not complicate the model I use a basic Logistic Regression Model for the task.
We use TfIdf vectorization to convert the content of our case statements to proper vectorized format where we use the top 5000 frequency word as the features. 
We then use a MultiLabelBinarizer for the task as it involves multi label outpu, to convert our tag data present in string format to a one hot encoder form for a multi Label Task.

Our model decent a good enough F1 score on validation set. If further optimized, it can also achieve much better performance.


#Run the colab

You can directly open the notebook from the 'open in colab' button on top of the notebook, the data requred is present in zip files, you dont need to unzip them manually as the program automatically unzips the given files.

The final result tags are also included in the 'predicted_tags.csv' file. 
