# 📘Litindex
![PyPI - Format](https://img.shields.io/pypi/format/Litindex?style=for-the-badge)
![Github-issues](https://img.shields.io/github/issues/cjenf/Litindex.svg?style=for-the-badge)

## This module is used to find old books.
> [!NOTE]
> **This project  provided by [openlibrary](https://openlibrary.org/).**<br>
> **Some books may not be found, please forgive me**
# Usage
```py
pip install Litinde
```
## Simple Example
```py
import Litindex
res=Litindex.Litindex(search="Pollyanna")
```
## Search for related books
```py
bookslist=res.books(page=1)
print(bookslist)
```
<details>
    <summary>See Example Output</summary>
    
```
[{'Pollyanna': 'https://openlibrary.org/works/OL2775807W?edition=key%3A/books/OL25265941M'}, {'Pollyanna': 'https://openlibrary.org/works/OL20789612W?edition=key%3A/books/OL29338558M'}, {'Study Guide: Pollyanna by Eleanor Hodgman': 'https://openlibrary.org/works/OL21868175W?edition=key%3A/books/OL38440931M'}, {'Pollyanna Grows Up': 'https://openlibrary.org/works/OL2775806W?edition=key%3A/books/OL37044774M'}, {'Pollyanna': 'https://openlibrary.org/works/OL17201497W?edition=key%3A/books/OL8133619M'}, {'Pollyanna': 'https://openlibrary.org/works/OL21617278W?edition=key%3A/books/OL51814456M'}, {'Pollyanna: Revised Edition': 'https://openlibrary.org/works/OL27106294W?edition=key%3A/books/OL39420010M'}, {'Pollyanna': 'https://openlibrary.org/works/OL36876696W?edition=key%3A/books/OL52170971M'}, {'Pollyanna': 'https://openlibrary.org/works/OL26293438W?edition=key%3A/books/OL36606576M'}, {'Pollyanna': 'https://openlibrary.org/works/OL31489360W?edition=key%3A/books/OL48234742M'}, {'Pollyanna': 'https://openlibrary.org/works/OL29551158W?edition=key%3A/books/OL46167182M'}, {"Pollyanna's jewels.": 'https://openlibrary.org/works/OL8645802W?edition=key%3A/books/OL13818142M'}, {'Pollyanna': 'https://openlibrary.org/works/OL20201422W?edition=key%3A/books/OL27555061M'}, {"Pollyanna's Western adventure.": 'https://openlibrary.org/works/OL8645806W?edition=key%3A/books/OL13789724M'}, {'Pollyanna: Large Print': 'https://openlibrary.org/works/OL29217912W?edition=key%3A/books/OL40188433M'}, {'Pollyanna & Pollyanna Grows Up': 'https://openlibrary.org/works/OL3069980W?edition=key%3A/books/OL11756048M'}, {'Pollyanna: Simplified Characters': 'https://openlibrary.org/works/OL37252084W?edition=key%3A/books/OL50214931M'}, {'Pollyanna: Audio CD': 'https://openlibrary.org/works/OL24228998W?edition=key%3A/books/OL32029176M'}, {'... Pollyanna in Hollywood': 'https://openlibrary.org/works/OL7641377W?edition=key%3A/books/OL6768688M'}, {"Eleanor H. Porter's Pollyanna": 'https://openlibrary.org/works/OL16053502W?edition=key%3A/books/OL24953431M'}]
```
</details>

```py
print(res.hit) # hits counts
>>> 272 hits
```

## methods
> [!NOTE]  
> ****the argument ```_title:str``` must come from ```books()```****

```res.title(_title="Eleanor H. Porter's Pollyanna")```
> **The title of the book**

```res.rate(_title="Eleanor H. Porter's Pollyanna")```
> **The rate of the book**

```res.author(_title="Eleanor H. Porter's Pollyanna")```
> **The author of the book**

```res.description(_title="Eleanor H. Porter's Pollyanna")```
> **The description of the book**

```res.publisher(_title="Eleanor H. Porter's Pollyanna")```
> **The publisher of the book**

```res.language(_title="Eleanor H. Porter's Pollyanna")```
> **The language of the book**

```res.pages(_title="Eleanor H. Porter's Pollyanna")```
> **The pages of the book**

```res.publish_date(_title="Eleanor H. Porter's Pollyanna")```
> **The publish_date of the book**

```res.series(_title="Eleanor H. Porter's Pollyanna")```
> **The series of the book**

