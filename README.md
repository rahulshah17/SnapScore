# SnapScore: A Novel NLP Technique to Evaluate Text-to-Image Models

## For LSTM
Using **LSTM_Image_Cap.ipynb** we have trained a model using LSTM and ResNet to caption images. The steps involved for training are as follows: 
* Import the MSCOCO dataset. 
* Create CNN encoder and RNN decoder we use a training routine to train the model and save it after training is complete.
* We load the model and generate captions for the test dataset.
* Then we calculated BLEU, ROUGE, Cosine, METEOR scores for computing snapscore.
* Three examples from the output of stable diffusion model are used for generating captions using the LSTM model.
* SnapScore of each of these generated captions is calculated by comparing it with a human annotated ground truth response.





## For Lavis
Using **NLP_Project.ipynb** we have trained a model using Lavis to caption images. The steps involved for caption generation are as follows:
* Three examples from the output of stable diffusion model are used for generating captions using the Lavis model.
* Then we calculated BLEU, ROUGE, Cosine, METEOR scores for computing snapscore.
* SnapScore of each of these generated captions is calculated by comparing it with a human annotated ground truth response.


We have compared the SnapScore for LSTM & Lavis in a tabular format in the report 

We have also computed graphs for Loss & Perplexity for every epoch in LSTM's training routine 


If you want to skip training and directly generate captions for custom images you can use the file **Saved_Model_Image_Captioning.ipynb** as it loads the saved model obtained by training LSTM.
