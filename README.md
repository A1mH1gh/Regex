# 업로드/다운로드 관련 키워드
다음은 upload, down, type="file", enctype="multipart", type:"file문자열을 포함하는 정규식입니다. 이 정규식은 대소문자를 구분하지 않고, 이 네 가지 키워드가 HTML 코드나 텍스트에서 등장하는지를 검사합니다
```
upload|down|type=\s["']file["']|type:\s["']file["']|enctype=["']multipart[^"']*["']
```

# Hidden 찾기 관련 키워드
다음은 <!--, //, display:none, visibility:hidden을 포함하는 문자열을 찾는 정규식입니다:
```
(<!--|\/\/|display\s*:\s*none|visibility\s*:\s*hidden)
```

# 3rd Party Library
## 1)
websquare
```
<debugMenu value="use"
```

# XSS
```
innerHTML()
/^javascript:(?!void\b).*/i
write()
outerHTML()
insertAdjacentHTML()
setAttrivute() //document.getElementById("target").setAttribute("onmouseover", "alert('XSS!')");
eval()
javascript:\s*[a-zA-Z_]+\([^()]+\)
```

# 개인정보
### 휴대폰번호
```
\d{2,3}-?\d{3,4}-?\d{4}
```

# 기타
## 1)
.png, .jpg, .gif, 또는 .ico가 포함된 문자열을 찾기 위한 정규식은 다음과 같습니다:
```
[a-zA-Z0-9_\-/]+\.(png|jpg|gif|ico|ttf|css)
```
"/test"
```
"([^"]+)"
```

"/..."
```
"\/[^"]+
```

(?<=name=")[^"]+
<input type="hidden" id="MsgId" name="MsgId" value="" />
MsgID

# 개발자도구
특정 확장자 제외
```
/^(?!.*\.(png|jpg|gif|svg|ico|css|woff|js)).*$/
```
