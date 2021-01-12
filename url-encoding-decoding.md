## URL 인코딩 & 디코딩
- URL 인코딩은 퍼센트 인코딩이라고도 불리며 URL에 문자를 표현하는 문자 인코딩 방법
- 알파벳이나 숫자 등 몇몇 문자를 제외한 나머지는 1바이트 단위로 묶인 16진수로 인코딩하는 방식
```python
from urllib import parse

# 인코딩
encode = parse.quote('한글')

# 디코딩
decode = parse.unquote('%ED%95%9C%EA%B8%80')

print(encode)
print(decode)

%ED%95%9C%EA%B8%80
한글
```