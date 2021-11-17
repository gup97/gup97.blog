---
title: 'VScode 메모장'
date: 2021-11-11 15:14:00
category: 'tip'
draft: false
---
vscode 관련기능을 적어 놓을 것
가끔 추가예정

- [vscode color thema 변경](#vscode-color-thema-변경)
- [javscript 가 prettier extension 적용이 안돼요](#javscript-가-prettier-extension-적용이-안돼요)

---

### vscode color thema 변경

F1 -> color Thema

---

### javscript 가 prettier extension 적용이 안돼요

ctrl + , -> `setting.json`
우측상단 `설정열기(json)` 클릭

```json
"[javascript]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
},
```

`setting.json` 에 위 코드 추가

---
