# Predicting the Stock Market?
This project examines the challenge of building machine learning models that can predict the rise and fall of the stock market based on what's in the news. For example, will stock prices rise with more positive 
news? Are there certain key phrases or words that impact the direction of market values? Are certain analytical approaches better for finding these relationships? 

Our analysis found:
* The stock market is too unpredictable to say that headlines can reliably predict market gains/losses. 
* Of the analysis techniques attempted, sentiment analysis came closest to providing signals for future stock market change over time.
* Of the topic modelling approaches used, Latent Dirichlet Allocation (LDA) provided better data for logistic regression analysis than Non-negative Matrix Factorization (NMF)...but both ultimately performed very poorly when attempting to predict stock market change.
* Topic models fitted to fast-changing data like news headlines become outdated quickly, and thus data pipelines should ensure that models are regularly being refitted.

## Built with
- [pandas](https://pandas.pydata.org/)
- [NLTK](https://www.nltk.org/)
- [scikit-learn](https://scikit-learn.org/stable/)
- [gensim](https://radimrehurek.com/gensim/)
- [matplotlib](https://matplotlib.org/)
- [plotly.js](https://plotly.com/javascript/)
- [Jupyter Notebook](https://jupyter.org/)

## A note on workflow
This analysis follows a specific workflow:
```
sentiment analysis and topic modeling on news headlines -> enhance existing data -> 
run regression and neural network models using headline topics and sentiments plus 
market gains/losses to find relationships
```
You'll want to explore the analysis notebooks in this general order:
1. Stock and news headline descriptive analysis
2. NLTK (sentiment analysis)
3. LDA / NMF (topic modeling) 
4. Logistic regression / recurrent neural networks

Notebooks containing Golden Cross and SVM analyses were used to help us understand performance benchmarks for market prediction techniques.

## Installation and use
### Download the repository
You can either download this repository as a zip file, or clone it locally using your favorite command line interface (typically Terminal on Mac or Git Bash on Windows) by running: 
```
git clone git@github.com:micahvandersteen/project-3-team-ifrit.git
```

### Exploring the data analysis notebooks
1. Install the necessary libraries via your CLI. Note: If you are an [Anaconda](https://www.anaconda.com/) user, you may have most of these libraries pre-installed. 
```
pip install pandas
pip install --user -U nltk
pip install jupyterlab
pip install -U scikit-learn
pip install gensim
python -m pip install -U matplotlib
```
2. Start a Jupyter Notebook by typing `jupyter notebook` in your CLI, then navigate to your desired notebook within the `Notebooks` folder of this repository. 
3. Open and run the notebook. 

### Interpreting the results
Analysis results and what they mean are described on the project webpage. 

## Contributors
- [Adam Bilski](https://github.com/abilski2013)
- [Alan Riveros](https://github.com/river127)
- [Brandon Uhler](https://github.com/buher8819)
- [Julia Revier](https://github.com/jrevier)
- [Katrina Koenders](https://github.com/katkoenders)
- [Micah Vandersteen](https://github.com/micahvandersteen)
- [Stacy Konkiel](https://github.com/skonkiel)

## Credits
Copyright for images included on the project webpage belongs to their respective owners.