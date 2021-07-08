# Napit
A naver Translate API Client

### Installation
Napit, short for 'Naver API Translate' is a tool to easily access the naver papago translator api. 
You can install this project with pip by running the command below.
```
pip install requests
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