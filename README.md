# Bookstore OOP

A small Python OOP exercise modeling a bookstore's inventory: books and coffee.

## Description

This project defines two classes:

- **`Book`** (`lib/book.py`) — has a `title` and `page_count`. The `page_count` property enforces that its value is an integer, printing `page_count must be an integer` otherwise. Calling `turn_page()` prints `Flipping the page...wow, you read fast!`.
- **`Coffee`** (`lib/coffee.py`) — has a `size` and `price`. The `size` property enforces that its value is `Small`, `Medium`, or `Large`, printing `size must be Small, Medium, or Large` otherwise. Calling `tip()` prints `This coffee is great, here's a tip!` and increases `price` by `1`.

## Installation

```console
$ pipenv install
$ pipenv shell
```

## Usage

```python
from lib.book import Book
from lib.coffee import Coffee

book = Book("Cradle", 200)
book.turn_page()

coffee = Coffee("Large", 3.50)
coffee.tip()
```

## Testing

Run the full test suite:

```console
$ pytest
```

Or run a single test file:

```console
$ pytest -x lib/testing/book_test.py
$ pytest -x lib/testing/coffee_test.py
```
