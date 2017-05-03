# Machine Learning Engineer Nanodegree
## Capstone Proposal
Michael Boker  
May 1st, 2017

### Domain Background
_(approx. 1-2 paragraphs)_

In this section, provide brief details on the background information of the domain from which the project is proposed. Historical information relevant to the project should be included. It should be clear how or why a problem in the domain can or should be solved. Related academic research should be appropriately cited in this section, including why that research is relevant. Additionally, a discussion of your personal motivation for investigating a particular problem in the domain is encouraged but not required.

### Problem Statement

The ability to predict changes in the stock market is a highly rewarding skill.  However, making these predictions can be quite challenging.  There is so much information to consider, that people must form large teams to try to analyze all of it quickly enough to keep up with market fluctuations.  This is a prime opportunity for machine learning to lend a hand.  The idea for this project is to use news headlines to predict market behavior.  Stock values are affected by many factors, but one of the most influential factors is public reaction to current events.  Deep learning methods could be useful for analyzing the news for a day, and predicting the resulting effect on the stock market.  Specifically, predictions would be made as to whether the values of stocks would rise or fall in a given day.  Ideally, models could be created for predicting the behavior of individual stocks, but this project will focus on one of the world’s most popular stock indexes. 

### Datasets and Inputs

The Dow Jones Industrial Average (DJIA) is a stock index, which incorporates the stock values of 30 of the largest companies in America.  An index is the average of a group of stocks.  It reflects the overall performance of that group.  The DJIA is commonly used as an indicator of the overall performance of the stock market as a whole.  The behavior of individual stocks is less predictable than that of a group of stocks, due to the effects of probability being more reliable with a group.  The DJIA would be a good source of information for testing the usefulness of deep learning in stock price prediction.  
	
A Kaggle dataset already exists for purposes similar to this project, and it contains data from 1990 days, ranging from the 8th of June, 2008 to the 1st of July, 2016.  This dataset pairs a collection of the top 25 news headlines from each day with a label indicating whether the DJIA rose or fell that day.  The news headlines are taken from the WorldNews subreddit, and are ranked based on user up-votes.  This seems to be a pretty good indicator that these are articles that the general public finds interesting.  Therefore, they are articles that are most likely to elicit a response from the public, which could have an effect on the DJIA.  This dataset can be found at https://www.kaggle.com/aaron7sun/stocknews.

### Solution Statement

Recurrent Neural Networks (RNN) are a popular deep learning technique for text analysis and can be powerful for sentiment analysis.  RNN’s can be used to learn context in a body of text, and not simply learn based on the words present in some text, as would be done with a simple feed-forward neural network and a bag of words.  For example, given a headline such as “United States Prepares to Wage War on Obesity,” an RNN would take the entire headline into consideration.  It might be able to determine that the phrase “Prepares to Wage War” is not referring to literal warfare.  A traditional feed-forward network would see the word “War” and probably determine that this article is about actual warfare, because it does not consider the surrounding context.  The long short-term memory (LSTM) model is a type of RNN, which is a particularly useful tool for sentiment analysis.  It can be used to learn from and predict on entire bodies of text, remembering the context of the entire piece as it goes along.  Other RNN’s have limits in the length of context that they can remember, due to problems encountered during back propagation when too much context is retained.  Therefore, an LSTM RNN will be used for this project.

### Benchmark Model
_(approximately 1-2 paragraphs)_

In this section, provide the details for a benchmark model or result that relates to the domain, problem statement, and intended solution. Ideally, the benchmark model or result contextualizes existing methods or known information in the domain and problem given, which could then be objectively compared to the solution. Describe how the benchmark model or result is measurable (can be measured by some metric and clearly observed) with thorough detail.

### Evaluation Metrics
_(approx. 1-2 paragraphs)_

In this section, propose at least one evaluation metric that can be used to quantify the performance of both the benchmark model and the solution model. The evaluation metric(s) you propose should be appropriate given the context of the data, the problem statement, and the intended solution. Describe how the evaluation metric(s) are derived and provide an example of their mathematical representations (if applicable). Complex evaluation metrics should be clearly defined and quantifiable (can be expressed in mathematical or logical terms).

### Project Design
_(approx. 1 page)_

In this final section, summarize a theoretical workflow for approaching a solution given the problem. Provide thorough discussion for what strategies you may consider employing, what analysis of the data might be required before being used, or which algorithms will be considered for your implementation. The workflow and discussion that you provide should align with the qualities of the previous sections. Additionally, you are encouraged to include small visualizations, pseudocode, or diagrams to aid in describing the project design, but it is not required. The discussion should clearly outline your intended workflow of the capstone project.

-----------

**Before submitting your proposal, ask yourself. . .**

- Does the proposal you have written follow a well-organized structure similar to that of the project template?
- Is each section (particularly **Solution Statement** and **Project Design**) written in a clear, concise and specific fashion? Are there any ambiguous terms or phrases that need clarification?
- Would the intended audience of your project be able to understand your proposal?
- Have you properly proofread your proposal to assure there are minimal grammatical and spelling mistakes?
- Are all the resources used for this project correctly cited and referenced?
