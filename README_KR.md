# Napit
네이버 파파고 통역 API 클라이언트

### 다른 언어
- [English](https://github.com/dolphin2410/napit/blob/main/README.md)

### 설치
'Naver API Translate'의 줄임말인 Napit은 쉽게 파파고 통역 API에 접근하는 것을 돕기 위한 파이썬으로 프로그래밍된 REST 클라이언트 입니다.
아래 명령어를 입력해 PYPI를 통해 다운로드 받으실 수 있습니다.
```
pip install napit
```
### 사용
```python
from napit.ApiRequest import ApiRequest
from napit.Credentials import Credentials
from napit.Languages import Language

# 네이버 개발자 어플리케이션 정보
credential = Credentials("CLIENT_ID", "CLIENT_SECRET")

# 안녕을 영어로 번역하고 출력합니다
print(ApiRequest.send(credential, Language.KOREAN, Language.ENGLISH, "안녕").text) 

```
### 공지
파이썬 처음 사용해 봐서 오류가 잦을 수 있습니다😂.
