# Movie Script Analysis 

This project involves advanced feature extraction from movie scripts and their analysis to identify correlations between said features and some success metrics. 

## Setup

### Python Dependencies

```
jupyter, networkx, gensim, sklearn, imdbpy
```

### Usage

Download the movie scripts from http://www.imsdb.com/ as shown below or directly download the database from [link].
```
@naman instruction for using the scraper
```
Extract scene and character details and store as jsons.
```
until finished
```

# Movie emotion/sentiment analysis

script: sentiment_bin.py
The script extracts sentiment/emotion from movie script in .txt format and 
provides sentiment/emotion quotient for the movie.

-------------------------------------INPUT----------------------------------
dirpath:    Directory where movie scripts are stored. (.txt format)
nrc_lex:    NRC lexicon for sentiment/emotion keywords (.csv format)
            Link to webpage: http://saifmohammad.com/WebPages/NRC-Emotion-Lexicon.htm
N:          Number of bins in which movie script is to be divided
------------------------------------OUTPUT----------------------------------
emotion_dict:   Dictionary with movie names as keys and doctionary of 
                sentiment/emotion quotient as values

The code first breaks script into N bins of equal number of lines. These bins 
are then processed for sentiment/emotion quotient based on keywords

Emotion quotient is obtained by normalizing word count by total word count of 
emotion words. Similarly for sentiment word count is normalized by total word 
count of sentiment keywords.

NB: Code fragment for pickling as has been commented. It can be used as desired
## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## References

* Vikas Ganjigunte Ashok, Song Feng and Yejin Choi, *Success with Style: Using Writing Style to Predict the Success of Novels*, EMNLP 2013 
* AM Dai, C Olah and QV Le, *Document embedding with paragraph vectors*, arXiv preprint arXiv:1507.07998 
* Gil, Sebastian, Laney Kuenzel and Suen Caroline, *Extraction and analysis of character interaction networks from plays and movies*,  CS 224W Final Project Report Sunday (2011). 
* Mohammad, Saif M. and Turney, Peter D., *Crowdsourcing a Word-Emotion Association Lexicon*, Computational Intelligence Vol. 29, 2013
* Q.V. Le and T. Mikolov, *Distributed Representations of Sentences and Documents*, ICML, 2014. arXiv:1405.4053 [cs.CL] 
* Mikolov, Tomas, Chen, Kai, Corrado, Greg, and Dean, Jeffrey, *Efficient estimation of word representations in vector space*, arXiv preprint arXiv:1301.3781, 2013a 
