IOD_project_3 
#[Ingredient Prediction with NLP & Machine Learning] (https://github.com/Aycrio/IODProject_3/tree/main)

This project delves into leveraging advanced multi-label classification techniques to analyze recipe directions, thereby providing shoppers with accurate ingredient predictions.

The dataset is obtained from Kaggle. (https://www.kaggle.com/datasets/paultimothymooney/recipenlg)

original data from:Bień, M., Gilski, M., Maciejewska, M., Taisner, W., Wisniewski, D., & Lawrynowicz, A. (2020). RecipeNLG: A Cooking Recipes Dataset for Semi-Structured Text Generation. In Proceedings of the 13th International Conference on Natural Language Generation (pp. 22-28). Dublin, Ireland: Association for Computational Linguistics. "https://www.aclweb.org/anthology/2020.inlg-1.4", pages = "22--28"


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
*   There were also tested on a recipe not found in the training data to identify the ingredients in the recipe directions

