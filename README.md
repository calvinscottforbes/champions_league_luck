champions_league_luck
==============================

Who are the luckiest teams in the Champions League?

Project Organization
------------

    ├── LICENSE
    ├── Makefile           <- Makefile with commands like `make data` or `make train`
    ├── README.md          <- The top-level README for developers using this project.
    ├── data
    │   ├── external       <- Data from third party sources.
    │   ├── interim        <- Intermediate data that has been transformed.
    │   ├── processed      <- The final, canonical data sets for modeling.
    │   └── raw            <- The original, immutable data dump.
    │
    ├── docs               <- A default Sphinx project; see sphinx-doc.org for details
    │
    ├── models             <- Trained and serialized models, model predictions, or model summaries
    │
    ├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                         the creator's initials, and a short `-` delimited description, e.g.
    │                         `1.0-jqp-initial-data-exploration`.
    │
    ├── references         <- Data dictionaries, manuals, and all other explanatory materials.
    │
    ├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
    │   └── figures        <- Generated graphics and figures to be used in reporting
    │
    ├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
    │                         generated with `pip freeze > requirements.txt`
    │
    ├── setup.py           <- makes project pip installable (pip install -e .) so src can be imported
    ├── src                <- Source code for use in this project.
    │   ├── __init__.py    <- Makes src a Python module
    │   │
    │   ├── data           <- Scripts to download or generate data
    │   │   └── make_dataset.py
    │   │
    │   ├── features       <- Scripts to turn raw data into features for modeling
    │   │   └── build_features.py
    │   │
    │   ├── models         <- Scripts to train models and then use trained models to make
    │   │   │                 predictions
    │   │   ├── predict_model.py
    │   │   └── train_model.py
    │   │
    │   └── visualization  <- Scripts to create exploratory and results oriented visualizations
    │       └── visualize.py
    │
    └── tox.ini            <- tox file with settings for running tox; see tox.readthedocs.io


--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>

# Who are the luckiest teams in modern Champions League?

## Intro

Sometimes when I watch the Champions league (and my favorite team loses of course) I do the normal things a fan does. There is no way that my team lost because they are a worse or they were outplayed. They lost because of LUCK! The other team was lucky, and we were the opposite. The winners of the tournament were lucky too. I decided to figure out if my (entirely rational) suspicions were correct.  

## Elements of Luck in the Champions League

### The Away Goal
My biggest gripe in the champions league is the away goal rule. I dispise it. You can look it up https://en.wikipedia.org/wiki/Away_goals_rule. It's an arbitrary way to decide who was the better side over two matches. My reasoning is that the two games are completely separate entities. Game 1 could be a high scoring affair while game 2 could be a 0-0 draw. The idea is that it's harder to score away goal. There is homefield after all right? I want to find out and test a few hypotheses.
1. Do teams actually score more at home than away?
2. Do teams that play at home first in a knockout round mathcup have a disadvantage? Is game 1 more likely to be high scoring?
3. Who has won the most from away goals? Who has lost the most?

### Random Draw
Many sports that I watch seed their tournaments (American perspective). Each team has a seed/ranking and that determines where they are placed in the tournament structure. This is not really the case with the Champions league or other European soccer tournaments. The group stages and the knockout rounds are often lopsided. To be fair, this happens in sports with seeding as well. The sometimes a team will make it to the finals without playing any of the top teams in the league. This is also an element of luck.

I want to find out what teams get the luckiest draws. How easy are their groups stages, and how easy are their knockout matchups? Finally, what champions have had the easiest runs to their titles?

## How I'm rankings teams
I decided to use the 5 year coefficients for teams. Essentially, they are the most straightforward way to get the ranking of a team.
I got my rankings from Kassiesa.net https://kassiesa.net/uefa/data/. This was the best way to get the coefficients. I wasn't able to find a database of them from UEFA (the governing body of the Champions league). Essentially these rankings grade the past performance in the UEFA competitions in the past 5 years. They also give a weight to the league they are in. A team from the Premiere League will get a better score than a team from the Turkish League. 

## 


# Update!

As I work on this project, UEFA decided to get rid of the away goal! https://www.uefa.com/returntoplay/news/026a-1298aeb73a7a-5b64cb68d920-1000--abolition-of-away-goals-rule-in-all-uefa-club-competitions/


