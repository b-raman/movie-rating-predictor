# Capstone Readme - Bharat Raman

## Included Files

    capstone_project.ipynb
    benchmark.ipynb
    Capstone_Report.pdf
    README.md

## Modules used:
#### Feature Engineering
    numpy - for arrays and other mathematical uses
    os - save and modify files in directories
    JSON - converting JSON format into list format for dataframe
    pandas - store and manipulate data in dataframe
    matplotlib.pyplot - plotting features to visualize feature to target relations

#### Training/Deploying/Evaluation Metrics

    sagemaker - accessing the estimator to train the model
    get_execution_role from sagemaker - For instantiating a role for training
    get_image_uri from  sagemaker.amazon.amazon_estimator - For accessing the XGBoost algorithm
    r2_score from sklearn.metrics - For calculating R^2 score for predictions

#### Hyperparameter Tuning

    IntegerParameter from sagemaker.tuner - describe the range of an integer hyperparameter
    ContinuousParameter from sagemaker.tuner - describe the range of a continuous hyperparameter
    HyperparameterTuner from sagemaker.tuner - used for creating hyperparameter tuning jobs in sagemaker

## References
- [5,000 movies from TMDb (kaggle dataset)][tmdb]
- [Benchmark Model by Ashwini Swain][k3]
- [Udacity Tutorials on Sagemaker Deployment][ud]
- [Sagemaker Documentation for XGBoost][xgb]
- [Scikit Learn Documentation for Evaluation Metrics][sklearn]
- [Sagemaker Documentation for Hyperparameter Tuner][hpt]
    


[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)


   [tmdb]: <https://www.kaggle.com/tmdb/tmdb-movie-metadata>
   [sklearn]: <https://scikit-learn.org/stable/modules/model_evaluation.html>
   [hpt]: <https://sagemaker.readthedocs.io/en/stable/tuner.html>
   [xgb]: <https://docs.aws.amazon.com/en_pv/sagemaker/latest/dg/xgboost.html>
   [ud]: <https://github.com/udacity/sagemaker-deployment/tree/master/Tutorials>
   [k3]: <https://www.kaggle.com/ash316/what-s-my-score>
   