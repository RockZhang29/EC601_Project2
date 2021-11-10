# EC601_Project2
This Project is EC601 Project 2.

About Twitter API program:

User Story 1: As a journalist, I want to use the Social Media Analyzer to realize what kinds of twitter do people like to post during their daily life, and build the flash-news by those topics who owning high sentiments.

User Story 2: As a commercial tenant, I want to retrieve the specific keywords, and using the sentiment tool to help me analyze the point of view that if they like the merchandise or it needs room for improvement.

Step 1: Create a Twitter account

Step 2: create an account for Tweepy and get permission to call.

step 3: copy the license password and pass the parameters.

step 4: call the API library function.

Step 5: Select a function in the API library for parameter call.

Step 6: create a new list and save API data to the list.

Step 7: use the fundction of Pandas to show something.

result: 
1. This API program is able to get access to my twitter account. 
2. It is able to show my timeline information. We can select the topic we want and print them.![c95325b8cc482e671560b35716788ae](https://user-images.githubusercontent.com/72896630/139682956-27f3f77c-7f1d-4db9-88b0-c23ab57ee735.png)

3. It is able to creat a form and show the data of the people I subscribe to.![966f6b5d084145f846e05aea2b0c265](https://user-images.githubusercontent.com/72896630/139682981-636f976e-cd0a-4bad-81e3-d70a229b5917.png)

4. It is also able to show the text of the subscriber.![71032f138ac345e8c345745d5be181d](https://user-images.githubusercontent.com/72896630/139682992-ebfbd4eb-5bf7-45ac-ac99-6bb8afaec8a9.png)


About Google NLP program:
Natural Language processing has a lot of branches. Sentiment analysis is one of them. Sentiment analysis can be defined as classifying text into different classes based on its texture. For gathering meaningful information from a text and use AI for classification use of IMDB dataset has been considered. IMDb reviews consist of 50,000 movie reviews in English (25,000 for training, 25,000 for testing) extracted from the famous Internet Movie Database, along with a simple binary target for each review indicating whether it is negative (0) or positive (1). This data set is very simple and has been decoded and preprocessed before. So, the input of training and testing for this data is number instead of alphabetic character. Labels of these reviews are stored as "0" and "1". For dealing with this classification task 2-layer GRU with 2 layers of dropout among them have been used. The structure of the models and their parameters has shown in Figure1. 
![微信图片_20211101095423](https://user-images.githubusercontent.com/72896630/139682850-d655bc7f-d0a7-47bc-b1c3-01aa4002d855.png)

Figure 1. Specification and information of model. Many of these reviews are very large and extracting negative or positive structure from them can be done only with the first 5 to 6 sentences. For example, this is one of the reviews for training: " This has to be one of the worst films of the 1990s when my friends I were watching this film being the target audience it was aimed at we just sat watched the first half an hour with our jaws touching the floor at how bad it was the rest of the time everyone else in the theatre just started talking to each other leaving or generally crying into their popcorn that they paid money they had earnt working to watch this feeble excuse for a film it must have looked like a great idea on paper but on film, it looks like no one in the film has a clue what is going on crap acting crap costumes I can't get across how embarrassing this is to watch save yourself an hour a bit of your life ". The negative meaning of these reviews can be seen from the first 3 sentences so there is no need to survey the rest. So, it had been decided to work with the first 300 words.

About the Model:

User Story:

Assume I'm a pollster and I want to see if there's more positive or negative tweets about the presidential candidates during the U.S. election campaign. To predict the who will win the election.

I created a model to extract API information and assess their emotional scores. The result is shown in the figure below: ![8638d7c387e1549813a5e45ee73205b](https://user-images.githubusercontent.com/72896630/139686393-4b7672ed-6d64-49b4-b0bf-362f367b4977.png)

We can see that this model carries out mean and variance operations on the emotional score of tweets.

For the Unit test, it is not easy for me to write a python test. So I would like to try it on Jupyter notebook. I wirte down some code to test my twitter API code.
