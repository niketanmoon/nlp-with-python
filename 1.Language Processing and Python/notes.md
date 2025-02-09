# Summary

## create virtual environment with pyenv

`pyenv virtualenv myEnv`

`pyenv activate myEnv`

## install jupyter

`pip install jupyter`

## install nltk

`pip install nltk`

## Downloading genesis context

`nltk.download('book')`

## Searching text with context

`concordance` can be used for this
`text1.concordance('wondered')`

## some other important functions

- `similar`: helps to find similar words
- `common_contexts`
- `generate`: Used for generating random texts
- `vocabulary`: `set(text1)`
- `vocabulary_size`: `len(set(text1))`
- `freq of word`: `text1.count('smote')`
- `FreqDist`: Method to find frequency distribution of a text

```
fdist = freqDist(text1)
```

- `fdist.most_common`: helps to find most common words in the given text
- `hapaxes`: gives single occuring words
- `collocations`: sequence of words that occurs together often

## Tokens and word types

`tokens` : text
`count of tokens`: len(text)
`word type`: set(text)
`count of word type`: len(set(text))
