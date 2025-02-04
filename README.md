# 7333-CaseStudy-2
QTW Case Study 2 - Diabetes 
The study linked explores the prediction of hospital readmission for diabetic patients using several machine learning models. 



Using a diabetes dataset to predict readmission within 30 days, I explore various models,  These models include: ogistic Regression, Random Forest, and a Stacking Classifier. This study focuses on addressing class imbalance (more non-readmitted than readmitted cases) using techniques like random undersampling (RUS) and SMOTE (Synthetic Minority Over-sampling Technique).  Key metrics used for evaluation include accuracy, macro-F1 score, weighted F1-score, and recall, with a particular emphasis on improving recall for the readmission class. My Jupyter Notebook details the data preprocessing steps, model training, hyperparameter tuning (especially for Random Forest), and a comparative analysis of model performance.

Key Takeaways:
- Stacking Classifier Excels in Recall: The Stacking Classifier emerges as the most effective model for predicting readmissions, particularly in maximizing recall (correctly identifying patients likely to be readmitted). This is crucial in a clinical context where minimizing missed readmissions is a priority.
- Random Forest Offers High Accuracy: Random Forest provides high overall accuracy but doesn't perform as well as the Stacking Classifier in terms of recall. This might make it suitable when a balanced measure of precision and recall is required.
- Class Imbalance Needs Addressing: The study highlights the importance of dealing with class imbalance, as it significantly impacts model performance, particularly the ability to detect the minority class (readmissions). Techniques like SMOTE proved effective in improving recall.
- Feature Engineering Plays a Role: The study emphasizes the impact of feature engineering and selection on model performance, suggesting further exploration in this area could yield even better results.

Overall:
This study provides a practical demonstration of applying machine learning to predict hospital readmissions for diabetic patients. It underscores the importance of considering metrics beyond just accuracy, particularly recall, in healthcare applications. The results highlight the effectiveness of ensemble methods like the Stacking Classifier in addressing class imbalance and improving prediction accuracy for the critical readmission class.


So what do the numbers say?
- The numbers in the study quantify the performance of the different machine learning models and demonstrate the impact of techniques like SMOTE. Here's what they tell us:
  Accuracy: Ranged from approximately 91% (Stacking Classifier) to 94% (Random Forest). While Random Forest had the highest overall accuracy, this metric alone doesn't tell the whole story, especially with imbalanced datasets.
- Macro F1-Score: Significantly higher for the Stacking Classifier (around 0.49) compared to Logistic Regression and Random Forest (both around 0.33). This indicates the Stacking Classifier's superior performance in balancing precision and recall across both classes (readmitted and not     readmitted).
- Weighted F1-Score: The Stacking Classifier achieved a very high score of approximately 0.91, demonstrating its effectiveness in handling the class imbalance and achieving good performance across both classes, weighted by their prevalence.
- Recall (Readmitted): While the exact numbers aren't provided directly in the summary, the study emphasizes that the Stacking Classifier achieved the highest recall for readmitted patients. This is the most critical metric in this context, as it reflects the model's ability to correctly identify patients at risk of readmission.
- Impact of SMOTE: The study indicates that SMOTE generally improved recall, but sometimes at the cost of slightly reduced precision. This highlights the trade-off between these two metrics, and the importance of finding the right balance based on the specific application.



In essence, the numbers show that while Random Forest had a slight edge in overall accuracy, the Stacking Classifier performed significantly better in identifying patients at risk of readmission (higher recall and macro-F1 score), especially when using SMOTE to address class imbalance. This makes the Stacking Classifier the preferred model when prioritizing the correct identification of potential readmissions.


** Note:  Lots ( too many if I'm being honest) other files and csv's are in the main QTW 7333 repo as I haven't yet moved them over, nor have I tidied the repositories.  Pardon the confusion.  One day, I might organize it(them).  But, not today, and probably not tomorrow.  

-JLTM  2-4-2025
-SMU MSDS Spring 2025 Quantifying The World
