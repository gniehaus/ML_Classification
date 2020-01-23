Classification Techniques to Determine Future Stock Price Performance

This project looked at stocks with a beta between .98 and 1.02 (follows the market) with the goal of trying to determine if the next day close would increase .3% compared to current day stock price. We use 19 securities (17 stocks and 2 indexes) with ~3900 days of trading.

All data was pulled from Bloomberg using an educational license. The data pulled matched data that can be pulled from Yahoo Finance, since I use webscraping to run predictions each day. This allows me to run the script on my local machine and get predictions without needing a Bloomberg terminal each day.

The machine learnings and analytics techniques used include: Data Wrangling, Regularization, Scaling, Feature Manipulation and Hyperparameter Tuning. Models used consist of: Support Vector Machines, K-Nearest Neighbors, Logistic Regression, and Random Forest. We predict labels and probabilities with LR, KNN, and RF.

Without additional computing power (enabling more stocks and features), the best models each predict proportionate to 0/1 labels. For instance, if 1500 rows predict tomorrow's price increase .3% and 1500 rows predict tomorrows price to not increase by .3%, the models predicts slightly better than .3%. As we change the proportion of the labels, the model's accuracy changes as well. Confusion Matrix is used to determine accuracy.

The result is 4 models that give predictions, with 3 giving probabilities. By combining the models predictions, we can better make trading decisions. This is a helpful start, but better predictive power can be reached.
