## [JavaScript] Copy non-circular-structure Object

> es6 기준


### 구조분해할당을 통하여 객체 복사를 할 수 있습니다.


```javascript
const a = {
  "b": 1,
  "c": 2,
  "d": "doodle"
};

const b = { ...a };
```

> JSON.stringify(a, null, 2)

```json
{
  "b": 1,
  "c": 2,
  "d": "doodle"
}
```

> JSON.stringify(b, null, 2)

```json
{
  "b": 1,
  "c": 2,
  "d": "doodle"
}
```

> JSON.stringify(a, null, 2) === JSON.stringify(b, null, 2)

```javascript
true
```

### 참고 자료

https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Operators/Destructuring_assignment

