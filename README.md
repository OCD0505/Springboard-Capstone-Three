Hold Steady: Keeping Your Donors

By utilizing donation records to develop predictive models, we now have a tool to enhance donor engagement and increase contributions for a nonprofit organization by analyzing donor lifetime value, predicting churn, and optimizing interactions based on donor history and demographics.

This dataset captures contributions data for small nonprofit organization since 2015 with all donor-identifying information removed for confidentiality purposes. To achieve working predictive models, several techniques were applied, such as imputation, encoding, vectorization, and hyper-parameter tuning. 

Project Organization
├── LICENSE
├── README.md          <- The top-level README for developers using this project.
├── data
│   ├── Links to Data.txt   <- Project data stored on Google cloud  
│       ├── data            <- Navigate to this using the Project Data Link within 'Links to Data.txt'
│             ├── interim   <- Intermediate data that has been transformed (Various versions available)
│                 
│                 └── Donations _ Jan 2015 to Mar 2024 R1 .csv	          <- Initial dataset (ie starting point) 
│                 └── Donations _ Jan 2015 to Mar 2024_R2 .csv	          <- 2nd revision of data during wrangling/cleaning
│                 └── Donations _ Jan 2015 to Mar 2024_R3 .csv            <- 3rd revision from applying feature engineering
│    
│             ├── processed  <- The final, canonical data sets for modeling.                                  
│                  └── Donations _ Jan 2015 to Mar 2024_R4_vectorized_encoded .csv           <- fully preprocessed data ready to train model
│                 
│                  
│             ├── raw    <- Data from third party sources
│                   └── Donations _ Jan 2015 to Mar 2024 R1 <- The initial, immutable data dump (revised for confidentiality purposes).   
│
├── docs               <- A default Sphinx project; see sphinx-doc.org for details
│
├── models             <- Trained and serialized models
│   ├── Links to Data.txt   <- pkl files stored on Google cloud  
│
├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
│                         the creator's initials, notebook name, project name and a short `-` delimited description, e.g.
│                         `1.0-jqp-initial-data-exploration-cap3`.
│
├── references         <- Data dictionaries, manuals, and all other explanatory materials.
│
├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
│   └── figures        <- Generated graphics and figures to be used in reporting
│
├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
│                         generated with `pip freeze > requirements.txt`
│
├── setup.py           <- makes project pip installable (pip install -e .) so src can be imported
├── src                <- Source code for use in this project.
│   ├── __init__.py    <- Makes src a Python module
│   │
│   ├── data           <- Scripts to download or generate data
│   │   └── make_dataset.py
│   │
│   ├── features       <- Scripts to turn raw data into features for modeling
│   │   └── build_features.py
│   │
│   ├── models         <- Scripts to train models and then use trained models to make
│   │   │                 predictions
│   │   ├── predict_model.py
│   │   └── train_model.py
│   │
│   └── visualization  <- Scripts to create exploratory and results oriented visualizations
│       └── visualize.py
│
└── tox.ini            <- tox file with settings for running tox; see tox.readthedocs.io

--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>
