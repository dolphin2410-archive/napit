# napit
Naver Translate API Client

Napit, short for Naver API Translate is a tool to easily access the naver papago feature. 
This project depends on 'requests'
```
pip install requests
```
```python
# Usage
import ApiRequest
from Credentials import Credentials
from languages import *

credential = Credentials(YOUR_CLIENT_ID, YOUR_CLIENT_SECRET)
print(ApiRequest.send(credential, Language.ENGLISH, Language.KOREAN, "Hello").text)  # 안녕
```
