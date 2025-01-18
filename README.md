# Smart Grid Stability Prediction Using Machine Learning

## Introduction
This project explores the stability of smart grids through the application of machine learning models. Unlike neural network approaches, our methodology emphasizes leveraging machine learning’s versatility and interpretability for analyzing tabular datasets. This approach enabled us to optimize computational efficiency and enhance predictive accuracy while analyzing grid stability factors.

The project builds on Paulo Breviglieri’s foundational insights, offering a distinct perspective by employing diverse classification algorithms, feature engineering techniques, and model interpretability tools.

Link to the <a href="https://www.kaggle.com/datasets/pcbreviglieri/smart-grid-stability/data">dataset</a>

---

## Renewable Energy Sources and Smart Grids
The rise of renewable energy sources has transformed traditional unidirectional energy flows into complex bidirectional systems, where ‘prosumers’ both consume and produce energy. These dynamics necessitate advanced methods for managing supply, demand, and economic implications within smart grids. Stability analysis plays a critical role in ensuring reliable energy management in this complex environment.

## Modeling Grid Stability
In smart grids, stability involves dynamically estimating and addressing energy production/consumption fluctuations. The project employs a binary classification model to predict grid stability ("stable" or "unstable") using parameters like power balance, reaction time, and price elasticity.

---

## Objectives
- Achieve high predictive accuracy for smart grid stability.
- Leverage machine learning algorithms for robust, interpretable solutions.

---

## Dataset
The dataset used is a synthetic simulation of grid stability in a 4-node star network. It includes 10,000 original observations, augmented to 60,000 through symmetry-based permutations. The dataset features:

### Predictive Features:
- **tau1** to **tau4**: Reaction times (0.5 to 10).
- **p1** to **p4**: Nominal power values (-2.0 to -0.5 for consumers).
- **g1** to **g4**: Price elasticity coefficients (0.05 to 1.00).

### Dependent Variables:
- **stab**: Maximum real part of the characteristic differential equation root.
- **stabf**: Binary stability label (“stable” or “unstable”).

The clean dataset requires no preprocessing, allowing for direct modeling.

---

## Methodology
### Training Techniques
1. **Standard Training**: Baseline method with data normalization.
2. **Correlation Matrix-Based Training**: Focused on influential features based on correlation analysis.
3. **K-Means Clustering-Based Training**: Enhanced dataset using cluster-based labels.
4. **Mutual Information Regression**: Feature selection based on mutual information scores.
5. **Principal Component Analysis (PCA)**: Dimensionality reduction to optimize performance.

### Models Employed
- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier
- XGBoost Classifier
- LightGBM Classifier
- And others (totaling 18 classifiers).

---

## Results
Key findings include:
- PCA and Mutual Information Regression achieved 100% predictive accuracy with Decision Tree, Random Forest, and XGBoost classifiers.
- Machine learning models offered superior interpretability and computational efficiency compared to neural networks.



---

## Conclusion
This project demonstrates the efficacy of machine learning in smart grid stability prediction, offering:
- Enhanced predictive accuracy (up to 100%).
- Improved interpretability and computational efficiency.
- Insights into renewable energy integration and grid management.

---

## References
1. Paulo Breviglieri, *Predicting Smart Grid Stability with Deep Learning* (2020).
2. Vadim Arzamasov, *Electrical Grid Stability Simulated Dataset*.
3. Arzamasov et al., *Towards Concise Models of Grid Stability* (2018).
4. Schafer et al., *Taming Instabilities in Power Grid Networks* (2016).
5. Léo Grinsztajn et al., *Why tree-based models outperform deep learning on tabular data* (2022).



