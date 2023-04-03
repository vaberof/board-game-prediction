# Predicting the probability of winning in the board game 'Codenames'

This project was created to participate in a scientific
student conference at ssugt as 
part of an artificial intelligence competition (took 1`st place). 
The main code source is in a board_game_prediction.ipynb

# Data

About 26,000 new rows of data were generated based on ~300 real 
collected data from the games after analyzing 
the factors influencing the victory 

# Models
### Linear Regression 
Results for the model:

Team 1 vs Team 2

|     MAE |    MSE |   RMSE |
|--------:|-------:|-------:|
| 3.75244 | 21.697 |  4.658 |

Team 1 vs Team 3

|     MAE |     MSE |    RMSE |
|--------:|--------:|--------:|
| 3.62246 | 20.3967 | 4.51627 |

Team 3 vs Team 2

|    MAE |     MSE |    RMSE |
|-------:|--------:|--------:|
| 4.3675 | 28.8067 | 5.36719 |

### Logistic Regression 
Results for the model:

Team 1 vs Team 2

|              |   precision |   recall |   f1-score |     support |
|:-------------|------------:|---------:|-----------:|------------:|
| 0            |    0.889417 | 0.908524 |   0.898869 | 1443        |
| 1            |    0.889076 | 0.866503 |   0.877644 | 1221        |
| accuracy     |    0.889264 | 0.889264 |   0.889264 |    0.889264 |
| macro avg    |    0.889246 | 0.887513 |   0.888256 | 2664        |
| weighted avg |    0.88926  | 0.889264 |   0.889141 | 2664        |

Team 1 vs Team 3

|              |   precision |   recall |   f1-score |     support |
|:-------------|------------:|---------:|-----------:|------------:|
| 0            |    0.892936 | 0.94344  |   0.917494 | 1715        |
| 1            |    0.88615  | 0.795574 |   0.838423 |  949        |
| accuracy     |    0.890766 | 0.890766 |   0.890766 |    0.890766 |
| macro avg    |    0.889543 | 0.869507 |   0.877958 | 2664        |
| weighted avg |    0.890519 | 0.890766 |   0.889326 | 2664        |

Team 3 vs Team 2

|              |   precision |   recall |   f1-score |     support |
|:-------------|------------:|---------:|-----------:|------------:|
| 0            |    0.868679 | 0.877265 |   0.872951 | 1214        |
| 1            |    0.896384 | 0.888966 |   0.892659 | 1450        |
| accuracy     |    0.883634 | 0.883634 |   0.883634 |    0.883634 |
| macro avg    |    0.882531 | 0.883115 |   0.882805 | 2664        |
| weighted avg |    0.883758 | 0.883634 |   0.883678 | 2664        |

