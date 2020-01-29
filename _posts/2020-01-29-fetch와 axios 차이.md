---
title: "fetch와 axios 차이"
date: 2020-01-29 11:55:25 -0400
categories: react fetch axios
---
1. Ajax 란?
AJAX (Asynchronous Javascript And Xml)

1. JavaScript를 사용한 비동기 통신, 클라이언트와 서버간에 XML 데이터를 주고받는 기술.
2. XMLHttpRequest 객체를 이용해서 전체 페이지를 리로드하지 않고 필요한 데이터를 로드할 수 있음.

2. Fetch (Ajax 구현방식1)
특징
javascript 내장 라이브러리이다. import 할 필요 x
return 값은 Promise 객체 형태.
```javascript
fetch('request url', {
  method: 'POST',
  body,
}).then((res) => {
  //...
});
```
3. Axios (Ajax 구현방식2)
특징
javascript 라이브러리 npm i axios
return 값은 Promise 객체 형태
```javascript
axios.post('request url', data)
  .then(function (res) {
    //...
  })
```