# News Caterorizer Demo

It's a logistic regression demo showed first time at my personal blog linked in description area.

Basically, it's a python program for command line that download and process some news content from brasilian sites and use scikit-learn Logistic Regression to classify them in some categories.

# Install

1. Clone the repo

2. Install requirements (I'm guessing you are using virtualenv):
```
$ pip install -r requirements.txt
```

3. Test instalation (It will show some help info)
```
$ python news_categorizer.py -h
```

# Use it

1. You need to download and process the news data:
```
$ python news_categorizer.py -f links.csv -t base.pkl
```

1.1 I'm providing you the file with several news links, but you can make yours!

1.2 When it finish you'll see something like that:
> Accuracy with 20% of testing data: 75%

2. Now you could classify some news links like that:
```
$ python news_categorizer.py -t base.pkl -p <link>
```