main.py README

How to run:
1) training set structure should look like: <br />
   <br />
external-detection-corpus-training/ <br />
├── source-document/ <br />
│   ├── part1/ <br />
│       ├── source-documentXXXXXX.txt (many more) <br />
├── suspicious-document/ <br />
│   ├── part1/ <br />
│       ├── suspicious-documentXXXXXX.txt (many more) <br />
<br />
2) change params 
MODEL = 'trigram'  # Choose 'unigram', 'bigram', or 'trigram'
MEASURE = 'cosine'  # Choose 'cosine' or 'jaccard'
DATASET = '/Users/walkertupman/Downloads/external-detection-corpus-training'
SOURCE_FOLDER = os.path.join(DATASET, 'source-document/part1')
SUSPICIOUS_FOLDER = os.path.join(DATASET, 'suspicious-document/part1')

^ example

3) run main.py