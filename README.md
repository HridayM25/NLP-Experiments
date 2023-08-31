# Question Answering Models 

Here are the notebooks I have made for exploring Question-Answering Models for a specific task. I have used the Haystack Model and SimpleTransformers Model, which I have trained on my custom dataset. 

This custom dataset was annotated through the features provided by Haystack, i.e Haystack Annotations. I had trained the models on about 150 such annotated questions and answers, based on my context.

In the second notebook, I have also incorporated Active Learning in the pipeline. More on Active Learning here : 

Whilst testing, answers which have a confidence score less than a certain threshold (0.65 as I have set it) need to be manually annotated and I am flagging all those instances. Whereas, answers with a higher confidence 
score are directly added to the training set and are incorporated in the pipeline, since the model worked relatively well on them. Hence this lessens the need for manual annotations, thus saving time and human effort.

I plan to further experiment with the threshold value to observe the results.
