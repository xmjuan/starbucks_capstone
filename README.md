# starbucks_capstone

### Project Introduction: 
This is the capstone project in Udacity Data Scientist Nanodegree Program.

### Library:
numpy <br>
pandas <br>
matplotlib.pyplot <br>
seaborn <br>
sklearn <br>
json <br>
math <br>
warnings <br>

### Motivation: 
This project uses Starbucks offer meta data to explore 'What is important to making an effective offer?'
It does EDA by answering some descriptive questions:
- Which offer type is the most difficult? Which reward is the most?
- Which offer type is completed the most?
- If number of completed offers differ by gender and age group?

### File description:
**Dataset:**
Portfolio.json: containing offer ids and features of each offer including reward, channels, difficulty, duration, offer type and unique offer id.
Profile.json: demographic data for each customer such as gender, age, date of becoming an member, income.
Transcript.json: records for transactions, offers received, offers viewed, and offers completed, presenting customers that got the offer, event info, value and time.
**Analysis:**
Starbucks_Capstone_notebook.ipynb

### Key process and results:
**Process:**
- Original data set is assessed, cleaned and explored.
- A new data set with effective offer label is created based on definition below:
when an offer id follows offer_received -> offer_viewed -> if transaction over offer difficulty -> offer_completed, it is regarded as an effective offer.
- New data set is assessed and explored.
- Model data set is created.
- Use several models e.g. random forest classifier, support vector machine, logistic regression, adaboost classifier and applied standard scaler to transform features.
- Tune parameters for adaboost classifier.
- Use model with best performance to assess feature importance.

**Results:**
Medium blog: https://medium.com/@juanximin/what-is-important-to-making-an-effective-offer-59dcedcef8fa

### Installation:
Python 3.7.10

### Author:
Ximin Juan

### Acknowledgements:
Udacity Data Scientist Program

### Reference:
https://towardsdatascience.com/the-ultimate-guide-to-adaboost-random-forests-and-xgboost-7f9327061c4f#:~:text=Compared%20to%20random%20forests%20and,being%20significantly%20slower%20than%20XGBoost.
https://moonbooks.org/Articles/How-to-manually-add-a-legend-with-a-color-box-on-a-matplotlib-figure-/