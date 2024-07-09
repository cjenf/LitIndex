# 📘Litindex
![PyPI - Format](https://img.shields.io/pypi/format/Litindex?style=for-the-badge)
![Github-issues](https://img.shields.io/github/issues/cjenf/Litindex.svg?style=for-the-badge)

### Search for books and various information about books
```py
pip install Litinde
```
# Simple Example
```py
import Litindex
res=Litindex.Litindex("Pollyanna")
```
# Search for related books
```py
bookslist=res.books(pages:int=1)
print(bookslist)
```
<details>
    <summary>See Example Output</summary>
```
[
```
