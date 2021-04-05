## ※ 문자사이 공백 없애기

- ### replace

: 문자열을 다른 문자로 대체 (공백을 ""로 대체하면 띄어쓰기 없애는 효과)

```js
const a = "Customer Service";

a.replace(/ /g, "");

//* 정규식에서 / /사이의 모든 값(g)을 두번째 인자로("")로 바꾼다.

//* 특정 문자를 바꿀 때 대소문자 가리지 않고 싶으면 g 뒤에 i붙일것.
```

- ### trim

: 문자열의 앞/뒤 공백을 제거한다.

```js
const a = " Customer Service ";

a.trim();
```
