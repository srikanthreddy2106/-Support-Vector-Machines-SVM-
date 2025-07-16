# -Support-Vector-Machines-SVM-

Support Vector Machines (SVMs) are powerful supervised learning models used for classification and regression tasks, renowned for their effectiveness in high-dimensional spaces. This analysis focused on employing SVMs for binary classification using a breast cancer dataset, aiming to distinguish between malignant and benign cases.

The process began with meticulous data preparation, including dropping irrelevant identifiers, encoding the categorical diagnosis column into a numerical format, and standardizing all features. The dataset was then split into training and testing subsets to facilitate model evaluation on unseen data.

We explored both linear and Radial Basis Function (RBF) kernels. Initially, the linear SVM demonstrated perfect accuracy on the test set, while the RBF kernel also performed strongly. To enhance robustness and prevent overfitting, particularly given the dataset's small size and class imbalance, hyperparameter tuning was conducted using GridSearchCV with StratifiedKFold cross-validation. This rigorous approach identified optimal C and gamma parameters, ensuring the models generalize well.

Furthermore, Principal Component Analysis (PCA) reduced the data to two dimensions, enabling clear visualization of the SVM decision boundaries. These plots distinctly illustrate how linear and non-linear kernels separate the classes, explicitly highlighting the crucial "support vectors"—the data points nearest to the hyperplane that dictate its position. Ultimately, the tuned linear SVM consistently outperformed the RBF kernel on this specific dataset, exhibiting strong classification capabilities.

Sources
