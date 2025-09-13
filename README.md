 # Poetry Language Model With LSTMs And Glove

 ## Overview
    + This project explores the use of a Long Short-Term Memory (LSTM) neural network to        generate poetry in the style of Robert Frost. 
    + The model is trained on a dataset of Frost's poems and utilizes pre-trained GloVe word embeddings to understand the semantic relationships between words.
    
    + **The Purpose of this project is to build a Poetry generation model:**
      * To determine how the model will generate next line of poem.
      * How it will make use of <sos> and <eos> tokens which forms the basis of Seq2Seq        Architecture.

 ## DataSet
    * The Dataset Used in this is the robert frost dataset which contains all the poems written by robert frost.

 ## Model Architecture
    * Embedding Layer-Transforms words into dense vectors.
    * <sos> tokens are used to make the model learn to start generating a sentence.
    * <eos> tokens are used to make the model learn to end generating a sentence at this token
    * A different sampling model is created as the model will only generate one word per time step.
 ## How to Run the code
    **To run this project, you will need to:**
      * Install Dependencies: Ensure you have the necessary Python libraries installed. The main libraries are TensorFlow, NumPy, and Pandas.
      * Download GloVe Embeddings: Download a pre-trained GloVe embedding file (e.g., glove.6B.50d.txt) and update the file path in the notebook. The current path is set to a specific location that you will need to change.
      * Run the Jupyter Notebook: Open the Poetry(LanguageModelling).ipynb notebook and run the cells sequentially.
    ** OR 
      * You can run this on Kaggle:-[Kaggle](https://www.kaggle.com/code/pranjalameta/poetry-generatrion-language-model)
 ## Results
    * The model's training history shows that the loss increases while the accuracy remains low. 
    * This also has to do with the fact that, In poem after "The" any word can come.
     
     