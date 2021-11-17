---
title: 같은 숫자는 싫어
date: 2021-11-11 14:11:03
category: algorithm
thumbnail: { thumbnailSrc }
draft: false
---
[프로그래머스 같은 문제는 싫어](https://programmers.co.kr/learn/courses/30/lessons/12906?language=javascript)

배열이 주어지면 중복된 숫자를 제거한 배열을 return  

---

## 처음 작성한 내 코드

```javascript
function solution(arr) {
  let result = [arr[0]];
  for (let i = 1; i < arr.length; i++) {
    if (arr[i - 1] != arr[i]) {
      result.push(arr[i]);
    }
  }
  return result;
}
```

> 입력 받은 배열의 전 값과 현재 값을 비교하여 다를 때마다  
새로운 배열 `result`에 추가해준다.

*멍청했다*  
예전 c언어했던 기억때문에 배열의 크기보다 높은 값을 사용하지 않으려고
1부터 시작하게 했는데 js에선 undefine으로 해결하면 됐다.
악습 하나를 고쳐야겠다.  

---

## 내가 보고 배울 코드들

### 1. filter 함수 사용

```javascript
function solution(arr)
{
    return arr.filter((val,index) => val != arr[index+1]);
}
```

>filter ( ) 활용한 코드  
이 함수는 알고 있었지만 활용할생각이 들지 않았다.  
[공부하자](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global_Objects/Array/filter)
