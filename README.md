IOD_project_3 
#[Ingredient Prediction with NLP & Machine Learning] (https://github.com/Aycrio/IODProject_3/tree/main)

This project delves into leveraging advanced multi-label classification techniques to analyze recipe directions, thereby providing shoppers with accurate ingredient predictions.

The dataset is obtained from Kaggle. (https://www.kaggle.com/datasets/paultimothymooney/recipenlg)

The ingredient binary matrix is created using nlp from the spaCy library on the ingredient column after cleaning and preprocessing steps

Model Training:
* The perfomance of 3 word vectorizers were compared using the OneVsRestClassifier(LogisticRegresion(solver='sag')) for the best performance
*   Tdif word level
*   Tdif n-gram level (uni-, bi-gram)
*   Word2Vec

* Then comparison of 3 machine learning models were compared for the best performance
*   LogisticRegression
*   RandomForestClassifier
*   XGBClassifier

* The metrics used to evaluate performance were:
*   Hamming loss
*   Micro-average F1 score
*   Macro-average F1 score
