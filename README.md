# English-to-Hinglish-translation
This Python script provides a simple English to Hinglish translation tool using the <a href="https://huggingface.co/docs/transformers/model_doc/marian">MarianMT</a> model from Hugging Face Transformers. It allows users to translate English sentences into Hinglish, a blend of Hindi and English, commonly used in informal communication.

To get started with the Hinglish translator,

- Clone this repository to your local machine:
   
   ```bash
   https://github.com/FozanAzhar/English-to-Hinglish-translation.git
   ```
- Install the required packages mentioned in the installation section.

  `pip install transformers`
  `pip install nltk`
  `pip install sentencepiece`
  
- Execute the notebook or run the script cells one by one.

## Approach

1. <b>Tokenization:</b> We tokenize the English text and identify nouns using the NLTK library.

2. <b>Translation:</b> Nouns are translated into Hindi, and the entire input text is translated using the Helsinki-NLP model.

3. <b>Hinglish Conversion:</b> The translated Hindi text is further transformed into a readable Hinglish version with consonant and vowel mappings.

4. <b>Noun Switching:</b> To maintain the essence of the text, we replace the translated nouns with their original English counterparts.

## Run the Translator

<img width="620" height="180" alt="stephinglish" src="https://github.com/FozanAzhar/English-to-Hinglish-translation/assets/95569589/fd204916-9cdd-4bba-825d-047b79298362">

## Sample Output
<img width="698" height ="90" alt="Hinglish output-1" src="https://github.com/FozanAzhar/English-to-Hinglish-translation/assets/95569589/dfe3a42c-d54e-4249-8d58-d2176f4db34d">

## Evaluating Model Performance

To evaluate the model's performance, you can use a variety of metrics depending on the specific use case.

- <b>Manual Evaluation:</b> Translate a set of English sentences to Hinglish and manually review the translations. Evaluate the quality of translations, correctness, and fluency.

- <b>BLEU Score:</b> Calculate the BLEU (Bilingual Evaluation Understudy) score to measure the similarity between the generated Hinglish text and reference translations. You can use NLTK's `nltk.translate.bleu_score` for this purpose.

- <b>Domain-specific Evaluation:</b> If the translation task is domain-specific (e.g., OpeninApp for Content creators), evaluate the model's performance within that specific domain.


