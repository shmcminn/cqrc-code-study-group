# Agenda

#### 1. Fire up a Jupyter notebook

#### 2. Go over what a Jupyter notebook does

#### 3. Strings, lists, dictionaries and booleans in Python

String: 
```python
"https://www.fbi.gov/file-repository/nics_firearm_checks_-_month_year.pdf/view"
```
List: 
```python
["https://www.fbi.gov/file-repository/nics_firearm_checks_-_month_year.pdf/view", "URL2"]
```
Dictionary (aka JSON): 
```python
{
"link": "https://www.fbi.gov/file-repository/nics_firearm_checks_-_month_year.pdf/view", 
"data_desc": "gun background checks", 
"maintainers": ["Sean", "Randy", "Ryan", "Sara", "Maite"]
}
```
Boolean: 
```python
gun_increase = True
```

#### 4. Go over libraries like `requests`

```python
import requests
url = "https://www.fbi.gov/file-repository/nics_firearm_checks_-_month_year.pdf/view"
response = requests.get(url)
print(response.text)
```
prints out:

```html
<!DOCTYPE html>
<html lang="en" data-gridsystem="bs3">
<head>
<meta charset="utf-8">
<meta http-equiv="x-ua-compatible" content="ie=edge">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>NICS Firearm Checks: Month/Year &#8212; FBI</title>
<meta name="DC.subject" content="CJIS, NICS, Firearms Checks">
<meta name="description" content="Statistics representing the number of firearms background checks initiated through the NICS from November 1998 to March 31, 2018.">
<meta name="DC.language" content="en-us">
<meta name="DC.date.created" content="2016-06-04T21:58:49+00:00">
<meta name="DC.description" content="Statistics representing the number of firearms background checks initiated through the NICS from November 1998 to March 31, 2018.">
<meta name="keywords" content="CJIS, NICS, Firearms Checks">
<meta name="DC.date.modified" content="2018-04-03T13:02:14+00:00">
<meta name="DC.format" content="application/pdf">
<meta name="DC.type" content="File">
<meta name="DC.date.valid_range" content="2016/06/04 - "> <link rel="canonical" href="https://www.fbi.gov/file-repository/nics_firearm_checks_-_month_year.pdf"><meta content="summary" name="twitter:card">
<meta content="NICS Firearm Checks: Month/Year">
...
```

#### 


