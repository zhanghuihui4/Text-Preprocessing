![text preprocessing](https://iq.opengenus.org/content/images/2019/09/text_preprocessing.PNG)

# Text-Preprocessing
Guidance and python code for text preprocessing

- # What is text preprocessing?
  Text preprocessing is a crucial step in natural language processing (NLP) and text analytics that involves preparing and cleaning textual data for analysis.
  
- # Why do we need text preprocessing?
  - The goal is to transform raw text into a format that can be easily understood and analyzed by algorithms or models.
  - Proper preprocessing can significantly enhance the performance and accuracy of subsequent tasks, such as text classification, sentiment analysis, and machine translation.
   
- # Text preprocessing techniques
  - **Text cleaning**
    - Lowercasing  
      Converting all characters in the text to lowercase.
        
    - Punctuation removal  
      Eliminate punctuation symbols like commas, periods, exclamation marks, etc.

    - Number removal  
      Depending on the analysis, numbers might not be relevant. In such cases, they can be removed.

    - Contraction expanding  
      Expand contractions, such as I'm, we'll, it's, etc.

    - Extra whiyte space removal
      Remove any extra spaces, tabs, or newlines.
  
  - **Stopwords removal**  
    Stopwords are common words (e.g., "and", "the", "is") that may not add significant meaning in analysis.
    ![stopwords](https://vectara.com/wp-content/uploads/2022/12/trashcan-wordcloud.jpg)
  
  - **Stemming & Lemmatization**
    - Stemming  
      Stemming is the process of reducing a word to its root form by removing suffixes (and in some cases prefixes) without understanding the context or using a dictionary.
      Example: Stemming "running" might return "run"; Stemming "flies" might return "fli".  
  

    - Lemmatization
      Lemmatization is the process of reducing a word to its base or dictionary form. It involves looking up a word in a lexicon and returning its lemma (canonical form).
      Example: Lemmatizing "running" might return "run"; Lemmatizing "better" with context might return "good".  

![stemming_lemmatization](https://media.licdn.com/dms/image/C4D12AQEZCHQOHXSEhg/article-cover_image-shrink_600_2000/0/1650689035153?e=2147483647&v=beta&t=uRsPEF-Apt9EvVTcUGR_ZhAs_Dk39de4MFQDo78LHos)


  - **Tokenization**  
    Tokenization is the process of converting a sequence of text (word/subword/sentence/character) into individual tokens, which are typically words, subwords, or phrases. These tokens become the basic units for text analysis.

![stemming_lemmatization](https://smltar.com/diagram-files/tokenization-black-box.png)

  - **POS tagging**  
    POS tagging involves assigning a part-of-speech label (e.g., noun, verb, adjective, adverb, etc.) to each token in a text based on its definition and its context in the sentence.  

    [Note]: It is better to keep the original text structure. Many words can have multiple POS tags depending on their context. For instance, "can" could be a modal verb ("I can swim") or a noun ("a can of soda"). Removing surrounding words, especially stopwords, can make it harder to disambiguate such cases.
		![POS tagging](https://1.bp.blogspot.com/-spGNcdlw7g4/XHY5fS25uVI/AAAAAAAABqY/63lfyQFHkl4rf1ls0vvLIBRRc8TEsBZvgCLcBGAs/s640/Capture.PNG)

  [Importance of POS tagging] 
  - **Syntactic Analysis**: Understanding the structure of a sentence and the relationships between words.
  - **Disambiguation**: Differentiating between words that have multiple meanings based on their usage. For example, in the sentence "I fish in the river," "fish" is a verb, but in "I caught a fish," "fish" is a noun.
  - **Enhancing Other NLP Tasks**: POS tags can improve the performance of tasks like named entity recognition, parsing, and machine translation.

  - **Segmentation**  
    Segmentation means the process of dividing a string of written language into its component words. This is especially important for languages where words are not separated by spaces, such as Chinese or Thai.

    Example: python package 'Jieba' for Chinese

    ![Segmentation](https://p1-tt.byteimg.com/large/pgc-image/8e739a6e052547c58343c306d8ac4fd7?from=pc)





      
