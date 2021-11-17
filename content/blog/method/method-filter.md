---
title: 'Array.prototype.filter()'
date: 2021-11-11 17:04:13
category: 'method'
draft: false
---
> [filter( )](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global_Objects/Array/filter) 메서드는 주어진 함수의 테스트를 통과하는 모든 요소를 모아 새로운 배열로 반환합니다.

## 2021-11-11

`filter()` 요약  
배열 내의 각 요소에 대하여 한번 제공된 `callback`함수를 호출해,  
`callback` 이 `true`로 구성된 배열을 생성함.
`callback`은 다음 세 인수와 함꼐 호출  

1. 요소값  
2. 요소 인덱스  
3. 순회되는 배열 객체

호출되는 배열을 변화시키지 않음  
`filter()` 호출 시작 이후 배열에 추가된 요소는 `callback`에 의해 방문되지 않는다.  

### 예시코드

```js
//10이하인 모든 요소 제거 , ture를 만족하는 값들로만 새로생성
var filtered = [12, 5, 8, 130, 44].filter(val => val >= 10);
```

```javascript
//연속된값 제거
function solution(arr)
{
    return arr.filter((val,index) => val != arr[index+1]);
}
```

---
