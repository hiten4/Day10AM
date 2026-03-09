# Day10AM
````markdown
# Python Dictionary Assignment

## Overview
This assignment demonstrates the use of Python dictionaries, defaultdict, and Counter to solve practical problems such as product catalog management, log analysis, and data processing.

---

## Part A — E-Commerce Product Catalog

A product catalog was created using nested dictionaries.

Structure:

```python
catalog = {
    sku: {
        "name": str,
        "price": float,
        "category": str,
        "stock": int,
        "rating": float,
        "tags": list
    }
}
````

Functions implemented:

* search_by_tag(tag) – find products with a specific tag
* out_of_stock() – list products with stock equal to 0
* price_range(min_price, max_price) – filter products by price range
* category_summary() – count, average price, and average rating per category
* apply_discount(category, percent) – apply discount to a category
* merge_catalogs(catalog1, catalog2) – merge two catalogs

Concepts used: dictionaries, dictionary comprehensions, defaultdict, and safe access using `.get()`.

---

## Part B — Log Analyzer

A simple server log analyzer was built.

Example log format:

```
2026-03-01 10:01:15 ERROR database Connection timeout
```

Features:

* Parse log entries into dictionaries
* Use Counter to find most common errors and active modules
* Use defaultdict to group errors by module
* Generate a summary report with total logs, error rate, and busiest module

---

## Part C — Interview Questions

**Dictionary Complexity**

* Lookup: O(1) average
* Insert: O(1) average
* Delete: O(1) average

Worst case can become O(n) due to hash collisions.

**Coding Problem**

Implemented a function to group anagrams using sorted words as keys and defaultdict(list).

**Debugging Task**

Fixed a character frequency function by:

* Using `.get()` to avoid KeyError
* Returning `(character, count)` pairs instead of only keys

---

## Part D — AI-Augmented Task

An AI-generated function was evaluated and improved.

The function merges two semester grade dictionaries and produces:

* Combined GPA
* Grade trend (improving, declining, stable)
* Subjects common to both semesters

Improvements added:

* Safe dictionary access using `.get()`
* Handling empty dictionaries
* Type hints and docstrings
* Cleaner and more Pythonic implementation

---

## Key Concepts

* Python dictionaries
* defaultdict and Counter
* Dictionary comprehensions
* Log parsing and analysis
* Data aggregation techniques

```
```
