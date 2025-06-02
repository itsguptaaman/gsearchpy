## 📦 gsearchpy 
**gsearchpy** is a lightweight Python package that allows you to perform Google Search queries programmatically and retrieve raw search result pages with ease.

It is built for developers, researchers, and automation enthusiasts who need a flexible interface to Google Search.

---

## Table of Contents

- [Features](#-features)
- [Installation](#-installation)
- [Example Usage](#-example-usage)


## 🚀 Features

- 🔍 Perform Google searches using customizable parameters  
- 📄 Retrieve raw HTML content and filtered data of Google search results  
- 🔁 Built-in pagination support  
---


## 📦 Installation

```
pip install gsearchpy
```

### Using Github
```
pip install git+https://@github.com/itsguptaaman/gsearchpy.git
```

### After Installation run this command to setup the drivers and dependency
```
gsearchpy
```


## 📦 Example Usage

### For raw data response 
```
from gsearchpy.google import google_search

query = "best VSCode extensions for productivity"
results = google_search(query)
```

### For clean data
```
from gsearchpy.google import google_search, filter_google_search_data

query = "best VSCode extensions for productivity"
html = google_search(query)
data = filter_google_search_data(html)
print(data)
```

### To get google maps data or any other data use tbm paramter
```
from gsearchpy.google import google_search

query = "best VSCode extensions for productivity"
results = google_search(query, tbm='lcl')
cleaned_data =extract_bussiness_data(results)
```

# Also you can use v2 except for google search you can use this for lcl, images, news, and etc.
```
from gsearchpy.google import google_search
results = google_search_v2("plumbers", page_number=2, gl="ahemdabad")
cleaned_data =extract_bussiness_data(results)
```

