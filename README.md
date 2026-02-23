# Web Page Parser

## Description
Part_1.py
This program takes a URL from the command line and:

* Fetches the web page
* Prints the page title
* Prints the page body text (without HTML tags)
* Prints all links present on the page

Part_2.py
This program compares two web pages to measure how similar they are.

It takes two URLs as input, downloads their content, extracts the body text, and counts the frequency of each word (case insensitive, alphanumeric only).

For every word, a 64-bit polynomial rolling hash is calculated. Using these hashes and their frequencies, the program computes a 64-bit SimHash for each page.

Finally, it compares the two SimHashes and prints how many bits are common out of 64. More common bits indicate higher similarity between the pages.

---

## Requirements

* Python 3
* requests
* beautifulsoup4

Install using:

```
pip install requests
pip install beautifulsoup4
```

---

## How to Run

Open terminal in the project folder and run:

```
python main.py <URL>
```

Example:

```
python main.py https://example.com
```


