Word Sense Disambiguation Using WordNet
1. Objective

The objective of this project is to identify the correct meaning of ambiguous words using WordNet and a Word Sense Disambiguation (WSD) algorithm.

2. Tools Used
Python
Google Colab
NLTK and WordNet
Pandas
3. Methodology

First, WordNet was used to retrieve the possible meanings, synonyms, definitions, and lexical relations of ambiguous words. Sample sentences containing the words bank, bat, and light were created. The Lesk algorithm was then applied to predict the intended sense based on sentence context.

4. Results

The system generated a sense inventory and a table of predicted word senses. Words such as bank can refer to a financial institution or the land beside a river. Similarly, bat can refer to an animal or a sports instrument. Context helps distinguish these meanings.

5. Conclusion

This project demonstrates a basic approach to Word Sense Disambiguation using WordNet. The Lesk algorithm provides a simple way to select a possible meaning for an ambiguous word. However, predictions may be incorrect when the sentence and WordNet definitions have few words in common. More advanced methods and manually annotated test data could improve performance.
