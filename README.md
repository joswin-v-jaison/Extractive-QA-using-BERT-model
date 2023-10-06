# Extractive-QA-using-BERT-model
This mini-project aims to perform question-answering on a given text passage using a pre-trained BERT-based model .The steps involved in the project can be summarized as follows:

1.Model Loading: The code loads a pre-trained BERT model.This model is capable of taking a question and a text passage as input and predicting the answer within the passage.

2.Tokenization: The input question and text passage are tokenized using the same tokenizer that was used during pre-training. This process converts the text into a format that the model can understand, including encoding the tokens as numerical IDs.

3.Segmentation: The code segments the tokenized input into two segments: one for the question and another for the text passage. This is necessary because BERT models are designed to handle multiple segments of text.

4.Model Inference: The tokenized and segmented input is passed into the loaded BERT-based model for inference. The model produces two sets of logits: start_logits and end_logits, which represent the likelihood of each position in the text being the start and end of the answer, respectively.

5.Answer Reconstruction: The code uses the logits to determine the predicted starting and ending positions of the answer span. It then reconstructs the answer span from the tokens, taking into account subword tokens (indicated by "##") and correctly formatting the answer.

6.Answer Output: Finally, the code prints the reconstructed answer to the console.

This mini-project showcases how a pre-trained BERT-based model can be used to perform question-answering tasks on text data. It demonstrates the tokenization, inference, and answer reconstruction steps necessary to extract answers from text passages given a question.
