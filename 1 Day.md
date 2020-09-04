# React&Typescript
우아한 테크러닝란 매주 화, 목 19:30~22:00까지 총 4주간 진행하는 React&Typescrip기반의 웹앱개발 강의이다.

올해는 코로나로 인해 온라인으로 진행하는 것이 아쉽다.

우아한 테크러닝의 3기로 뽑혀 React와 Typescript를 배울 수 있는 기회를 얻게 되어서 정리를 하게 되었다.

우아한형제들의 웹프론트앤드개발그룹장인 김민태님께서 진행해주신다. 

## TypeScript type을 기술하는 두 가지 방법 (Type Alias, Interface)
TypeScript는 변수명 뒤에 타입을 명시하는 것으로 타입을 선언할 수 있다.

``` js
let foo1 : Number= 10;    //명시적
let foo2 = 10;            //추론적
foo2 = false;             //오류 발생
```
위와 같이 `JavaScript`와 동일하게 코드를 작성할 수 있다.

타입추론을 통해 오류를 발생시키지 않는다.

하지만 `foo2`변수에 `Number` 타입이 지정되면 다른 타입의 값은 대입할 수 없다.

명시적으로 타입을 지정해도 다른타입의 값은 대입할 수 없다.

추론적인 코드보다는 **명시적인 코드가 직관적이고 읽기 쉽다.**

### Type Alias
Type Alias(타입 별칭)는 타입에 직접 이름을 부여할 수 있다.

``` js
type Age = Number;      //TypeAlias 사용

let age : Age = 10;
let wight : Number = 80;
```
타입 별칭을 통해 **가독성을 증가**시킬 수 있다.

### Interface
interface를 알기 위해선 객체 타입을 알아야한다.

객체의 타입은 `Type` 키워드를 사용해 정의할 수 있다.
``` js
Type Foo = {
  age : number,
  name : string;
}

const foo : Foo = {
  age : 10,
  name : "Kim"
}
``` 
` Foo`  객체의 타입은 ` number` 타입과 ` string` 타입을 가지고 있다.

``` js
type Age = number;

interface Bar {
  age : Age,
  name : string;
}

const bar : Bar = {
  age : 10,
  name : "Kim";
}
```


## React의 엘리먼트, 컴포넌트, ReactDom.render


#### 수업 참조 링크
- [TypeScript Code 테스트 공간]()
- [통합 IDE](https://codesandbox.io/index2)
- [React 라이브러리](https://reactjs.org)
- [Redux 상태 관리 라이브러리](https://redux.js.org)
- [CSS UI 라이브러리](https://blueprintjs.com)
- [테스트 공간](https://testing-library.com)
