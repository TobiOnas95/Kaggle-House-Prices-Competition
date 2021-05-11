# Kaggle-House-Prices-Competition

The code in this repository is my submission to the Kaggle House Prices Competition.
It is a regression problem and my submission earned me a place in the top 2% of all submissions to the competition. 
My kaggle profile can be viewed using the link below:
https://www.kaggle.com/tobionasanya 

I have added some notes on the code in certain cells to explain some choices I made, I think this would be beneficial to understanding the code.

Cell [7]: Mutual Information (MI) is used to determine the features to develop and also features that will not contribute. MI between two quantities
          is a measure of the extent to which knowledge of one quantity reduces the uncertainty about the other. 

Cell[11]: Different features we're created and the score of the model with the new feature is compared to the score in cell [10]. Features that improved 
          the model are tagged "#good" and ones that dont are tagged "#not good". 

Cell [13]: Principal Component Analysis (PCA) is an unsupervised model used here for feature creation. It is used to decompose the variational structure 
           in the data. The PCA algorithm provides us with loadings which gives insight into each component of variation, and this was used to suggest 
           features to create. 

Cell [23]: This function makes it possible to target encode without having to hold out encondint data which leading to waste. It is the same principle as 
           cross-validation. The data is initially split into folds, each fold has two splits of the dataset. The encoder is trained on one split while 
           the values of the other are transformed. This is then repeated for all the splits. 


