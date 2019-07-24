## [JavaScript] Copy

> es6 기준


### 구조분해할당 방법

> 단, 완전한 깊은 복사는 아닙니다. 멤버 중 배열, 객체는 참조복사가 적용됩니다.

```javascript
const a = {
  "b": 1,
  "c": 2,
  "d": "doodle"
};

const b = { ...a };
```


### JSON 방법

> 깊은 복사지만, stringify 후 parse 하는 방법으로 큰 객체의 경우 매우 느릴 수 있습니다.

```javascript
const a = {
  "b": 1,
  "c": 2,
  "d": "doodle"
};

const b = JSON.parse(JSON.stringify(a));
```


### 참고 자료

https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Operators/Destructuring_assignment


