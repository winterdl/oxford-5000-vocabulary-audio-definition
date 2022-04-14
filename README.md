# English vocabulary + pronounciation + definition

This project aims to provide easy-to-read and printable vocabulary list of the
most common words of the English language with their meaning.

The lists are mostly based on data gathered from the oxford 3000, 5000 and 5000 exclusive lists.

The word lists contain the following points of data
* Spelling (text)
* Pronounciation (audio)
* Lexical spelling (text)
* Meaning (text)
* Example (text)

You can find  data in `/data` in formats `.pkl`, `.csv`, `.json`
Audio (10K files, 200MB) are archived in `.zip` files in `/audio`

Lists in `/output` are formatted alphabetically, by CEFR rating, random and viewable in
`.pdf` and `.html` format.

TODO Audio integration 

## Folder structure
```
├── audio
│   ├── *_uk.mp3
│   ├── *_us.mp3
│   ├── ...
├── data
│   ├── df_concat.pkl
│   ├── df_definition.pkl
│   ├── df.pkl
│   ├── oxford_3000.csv
│   ├── oxford_3000.json
│   ├── oxford_3000.pkl
│   ├── oxford_5000.csv
│   ├── oxford_5000_exclusive.csv
│   ├── oxford_5000_exclusive.json
│   ├── oxford_5000_exclusive.pkl
│   ├── oxford_5000.json
│   └── oxford_5000.pkl
├── output
│   ├── oxford_3000_alphabetical.html
│   ├── oxford_3000_alphabetical.pdf
│   ├── oxford_3000_by_cefr.html
│   ├── oxford_3000_by_cefr.pdf
│   ├── oxford_3000_two_column_alphabetical.pdf
│   ├── oxford_3000_two_column_by_cefr.pdf
│   ├── oxford_5000_alphabetical.html
│   ├── oxford_5000_alphabetical.pdf
│   ├── oxford_5000_by_cefr.html
│   ├── oxford_5000_by_cefr.pdf
│   ├── oxford_5000_exclusive_alphabetical.html
│   ├── oxford_5000_exclusive_alphabetical.pdf
│   ├── oxford_5000_exclusive_by_cefr.html
│   ├── oxford_5000_exclusive_by_cefr.pdf
│   ├── oxford_5000_exclusive_two_column_alphabetical.pdf
│   ├── oxford_5000_exclusive_two_column_by_cefr.pdf
│   ├── oxford_5000_two_column_alphabetical.pdf
│   └── oxford_5000_two_column_by_cefr.pdf
├── format.ipynb
├── scrape.ipynb
```
## Scraping
Selenium, beautifulsoup, requests, pandas

See `scrape.ipynb`

## Formatting
Data in pandas dataframe

df ---pandas---> HTML ---pandoc---> pdf

df ---pandas---> tex ---LaTeX---> pdf

See `format.ipynb`

## Resources and credit
Oxford 5000 list, online interface to lookup words, filter by CEFR level,
listen pronounciation (US,UK)
also shows meaning but only after clicking to a new page.
https://www.oxfordlearnersdictionaries.com/wordlists/oxford3000-5000

dictionary by tusharlock10
https://github.com/tusharlock10/Dictionary
with relevant stackoverflow thread
https://stackoverflow.com/questions/41768215/english-json-dictionary-with-word-word-type-and-definition
