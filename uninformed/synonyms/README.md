# Synonym Substitution

The script generate_sysnonyms.py takes as input a set of articles and outputs a new set of articles, in which words have been changed
to their synonyms (the first article in the new set has one word changed, the next article has two words changed, etc.). The new articles
have a new JSON element, 'numSyns'. which is simply the number of synonyms present in the article. Synonyms are generated using the
[NLTK wordnet](https://www.nltk.org/).

To install NLTK Wordnet:
1. in the anaconda prompt, run `pip install nltk`
2. Run the python shell and enter two commands, `import nltk` and `nltk.download()`. This will open the nltk downloader
3. In the downloader, select "Corpora" and scroll down to "Wordnet". Click download.

Then, call `python generate_synonyms.py <input json file> <output json file>` to generate the synonyms.

