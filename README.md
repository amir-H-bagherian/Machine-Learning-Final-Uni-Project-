# Machine-Learning-Final-Uni-Project-

## Intro
This is the final university project with thesis pdf file. This project uses XGBoost &amp; LightGBM models to classify breast cancer patients into Benign &amp; Malignant classes.

## XGBoost
Because of time-intensivity optimization processes, first the optimal values for learning_rate and n_estimators params calculated (0.27 & 157 respectively). Then the other params optimized using the optimal values of the two mentioned params.
> The final result may not be the best optimum, but since processing all combinations of different values for all params took too long to finish; The Search Space pruned and the provided model with provided params is achieved.

## LightGBM
Again because of time-intensivity optimization processes, first the optimal values for learning_rate and n_estimators params calculated (0.19 & 149 respectively). Then the other params optimized using the optimal values of the two mentioned params.
> The final result may not be the best optimum, but since processing all combinations of different values for all params took too long to finish; The Search Space pruned and the provided model with provided params is achieved.

## LightGBM with Optuna
Optuna is an optimization framework which find the optimal hyperparams very quickly. This framework is used on LGBM only because of lack of time in preparing thesis for university. You may use it for XGBoost too.
There is an objective function for optimization process which is passed to an `optuna.study` object to maximize its output (i.e. return value). This is set to be done in 100 rounds of optimization.<br>
Obtained result is not as good as the result of customized LGBM implementation in the other LGBM-implementation file; But it is still better than LGBM model trained on default values.

<br>
ROC Curve and PR Curve along side some SHAP models are drawn in all 3 implementation files.
