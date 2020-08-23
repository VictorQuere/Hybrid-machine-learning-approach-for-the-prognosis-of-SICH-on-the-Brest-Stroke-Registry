# Hybrid-machine-learning-approach-for-the-prognosis-of-SICH-on-the-Brest-Stroke-Registry
Travail de mémoire de master 2 Neurosciences Cliniques de Rennes

Abstract :

Background : Spontaneous Intracerebral Hemorrhages (SICH) account for one to two million cases per year worldwide with a severe prognosis and without any specific therapy having shown benefits. Prognostic tools are useful to facilitate streamline assessment, communication between providers and may contribute to the emergence of new therapeutic studies. Current tools lack of transparency, precision and do not take into account missing data. However, there are solutions using machine learning that meet these criteria. Consequently, the objective of this study was, without excluding missing data, to develop a powerful machine learning model which efficiently describes each step of the decision, while remaining interpretable.

Methods : We worked on data from the population-based Brest Stroke Registry from 2008 to 2017. Demographic, related to medical history, clinic, laboratory and imaging data were considered as interesting variables to assess mortality at 30 days. Missing data were imputed either by a one-hot method or the median of observations. We performed variables selection using mean decrease in Gini from a classification and regression tree (CART). Then, after dividing the data into training and testing sets, we performed a clustering using a K-means algorithm. Finally, we trained and optimized a support vector machine (SVM) for each cluster. The overall model was evaluated using the area under the ROC curve (AUC), accuracy, recall and F1 score.

Results : The data of 1077 validated cases of SICH, were included. 18 variables were analyzed. Of these, eight (SICH volume, glucose, history of RANKIN score, age, Glasgow score, NIHSS, systolic and diastolic blood pressure) were selected using a CART. In addition to Glasgow score and SICH volume, NIHSS and glucose were found to be informative. According to the results of elbow method, data were divided into four groups during the clustering step. Among the clusters, two had characteristics not yet described in the literature. After training the SVMs, the overall AUC of the model was 0.75, the accuracy 0.74, the recall 0.81 and the F1 score 0.77.

Conclusions : We have developed, without excluding missing data, an easily explainable machine learning model to predict 30-day mortality from SICH. Preliminary results showed that high NIHSS and glucose appear to be linked to poor prognosis. Moreover, we described a group of patients with high blood pressure on which it would be interesting to conduct therapeutic studies. Although comparison was not possible, the overall performance appears to be inferior to the previous models.
