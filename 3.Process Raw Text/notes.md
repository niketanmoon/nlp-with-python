## Getting html data from link
```
from urllib.request import urlopen
raw = urlopen(url).read().decode('utf-8')
```

## The NLP Pipeline
- HTML --> ASCII --> Text --> Vocab
- HTML
    - html = urlopen(url).read().decode('utf-8')
    - soup = BeautifulSoup(html, 'html.parser')
    - raw = soup.get_text()
- ASCII
    - tokens = nltk.wordpunct_tokenize(raw)
- Text    
    - text = nltk.Text(tokens)
- Vocab
    - words = [w.lower() for w in text]
    - vocab = sorted(set(words))


## Stemming and Lemmatization
- Both aims to reduce the word to their base form but lemmatization takes context into account to produce a recognized dictionary word called as lemma