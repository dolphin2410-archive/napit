# Napit
A naver Translate API Client

### Other Languages
- [Korean](https://github.com/dolphin2410/napit/blob/main/README_KR.md)

### Installation
Napit, short for 'Naver API Translate' is a client programmed with python that allows you to easily access the naver papago translator api. 
You can install this project with pypi by running the command below.
```
pip install napit
```
### Usage
```python
from napit.ApiRequest import ApiRequest
from napit.Credentials import Credentials
from napit.Languages import Language

#Your API Credentials
credential = Credentials("CLIENT_ID", "CLIENT_SECRET")

# Translates 'Hello' from english to korean
print(ApiRequest.send(credential, Language.ENGLISH, Language.KOREAN, "Hello").text) 

```
### Notice
I learned python in a day and this is my first project with python. There might be lots of errors 😂.
