# Heat-Exchanger-Prediction

This repository contains the data and codes used in the experimental part of the paper “A prediction model for heat exchanger fouling factor based on stacking model” by Zhiping Chen, Yongle Meng et al.

## Abstract
Given the pressing demand for energy conservation, the petrochemical sector faces increasingly stringent energy-saving mandates. Heat exchangers, essential to this sector, suffer efficiency losses and increased energy consumption due to fouling. To ensure optimal operation of heat exchange systems, regular assessment of solid deposits and the implementation of cleaning schedules are imperative. However, the multitude of influencing factors renders traditional estimation methods unreliable. Consequently, we developed a stacking model to predict the fouling factor  of heat exchangers. Specifically, we first constructed fouling factor prediction models using various machine learning techniques, then selected the best-performing models—random forest, extreme gradient boosting , and light gradient boosting machine—for integration. Finally, the predictions from these three models were fed into a linear regression layer to form the final stacking model. The results indicate that the constructed stacking model significantly enhances the accuracy of fouling factor prediction. This model not only surpasses traditional multilayer perceptron neural network methods but also outperforms the well-performing gaussian process regression. This achievement not only validates the effectiveness of our model but also provides robust support for future research and applications in related fields.

## Code and data
all.ipynb and stacking.ipynb are our codes
data.xlsx is the data we use

## Experimental Results


         Performance comparison of classical ML prediction models.
| Methods       | MSE          | MAE          | MAPE% | R²     | RAE% |
|---------------|--------------|--------------|-------|--------|------|
| Knn           | 6.94 × 10⁻⁴  | 7.08 × 10⁻³  | 19.19 | 0.98029| 4.63 |
| Random forest | 1.30 × 10⁻⁴  | 4.40 × 10⁻³  | 16.68 | 0.99631| 2.87 |
| Bagging       | 1.54 × 10⁻⁴  | 4.80 × 10⁻³  | 16.06 | 0.99561| 3.13 |
| Xgboost       | 1.65 × 10⁻⁴  | 4.82 × 10⁻³  | 16.23 | 0.99617| 3.09 |
| Lightgbm      | 1.50 × 10⁻⁴  | 4.34 × 10⁻³  | 16.59 | 0.99622| 3.28 |
| GPR           | 4.50 × 10⁻⁴  | 5.18 × 10⁻³  | 16.21 | 0.99221| 5.81 |
