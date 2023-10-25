- [19장 프로토타입](#19장-프로토타입)
- [19.1 객체 지향 프로그래밍](#191-객체-지향-프로그래밍)
  - [19-01](#19-01)
  - [19-02](#19-02)
- [19.2 상속과 프로토타입](#192-상속과-프로토타입)
  - [19-03](#19-03)
  - [19-04](#19-04)
- [19.3 프로토타입 객체](#193-프로토타입-객체)
  - [19.3.1 `__proto__` 접근자 프로퍼티](#1931-__proto__-접근자-프로퍼티)
    - [19-05](#19-05)
    - [19-06](#19-06)
    - [19-07](#19-07)
    - [19-08](#19-08)
    - [19-09](#19-09)
    - [19-10](#19-10)
  - [19.3.2 함수 객체의 prototype 프로퍼티](#1932-함수-객체의-prototype-프로퍼티)
    - [19-11](#19-11)
    - [19-12](#19-12)
    - [19-13](#19-13)
  - [19.3.3 프로토타입의 constructor 프로퍼티와 생성자 함수](#1933-프로토타입의-constructor-프로퍼티와-생성자-함수)
    - [19-14](#19-14)
- [19.4 리터럴 표기법에 의해 생성된 객체의 생성자 함수와 프로토타입](#194-리터럴-표기법에-의해-생성된-객체의-생성자-함수와-프로토타입)
  - [19-15](#19-15)
  - [19-16](#19-16)
  - [19-17](#19-17)
  - [19-18](#19-18)
  - [19-19](#19-19)
- [19.5 프로토타입 생성 시점](#195-프로토타입-생성-시점)
  - [19.5.1 사용자 정의 생성자 함수와 프로토타입 생성 시점](#1951-사용자-정의-생성자-함수와-프로토타입-생성-시점)
    - [19-20](#19-20)
    - [19-21](#19-21)
  - [19.5.2 빌트인 생성자 함수와 프로토타입 생성 시점](#1952-빌트인-생성자-함수와-프로토타입-생성-시점)
    - [19-22](#19-22)
- [19.6 객체 생성 방식과 프로토타입의 결정](#196-객체-생성-방식과-프로토타입의-결정)
  - [19.6.1 객체 리터럴에 의해 생성된 객체의 프로토타입](#1961-객체-리터럴에-의해-생성된-객체의-프로토타입)
    - [19-23](#19-23)
    - [19-24](#19-24)
  - [19.6.2 Object 생성자 함수에 의해 생성된 객체의 프로토타입](#1962-object-생성자-함수에-의해-생성된-객체의-프로토타입)
    - [19-25](#19-25)
    - [19-26](#19-26)
  - [19.6.3 생성자 함수에 의해 생성된 객체의 프로토타입](#1963-생성자-함수에-의해-생성된-객체의-프로토타입)
    - [19-27](#19-27)
    - [19-28](#19-28)
- [19.7 프로토타입 체인](#197-프로토타입-체인)
  - [19-29](#19-29)
  - [19-30](#19-30)
  - [19-31](#19-31)
  - [19-32](#19-32)
  - [19-33](#19-33)
  - [19-34](#19-34)
  - [19-35](#19-35)
- [19.8 오버라이딩과 프로퍼티 섀도잉](#198-오버라이딩과-프로퍼티-섀도잉)
  - [19-36](#19-36)
  - [19-37](#19-37)
  - [19-38](#19-38)
  - [19-39](#19-39)
- [19.9 프로토타입의 교체](#199-프로토타입의-교체)
  - [19.9.1 생성자 함수에 의한 프로토타입의 교체](#1991-생성자-함수에-의한-프로토타입의-교체)
    - [19-40](#19-40)
    - [19-41](#19-41)
    - [19-42](#19-42)
  - [19.9.2 인스턴스에 의한 프로토타입의 교체](#1992-인스턴스에-의한-프로토타입의-교체)
    - [19-43](#19-43)
    - [19-44](#19-44)
    - [19-45](#19-45)
- [19.10 instanceof 연산자](#1910-instanceof-연산자)
  - [19-46](#19-46)
  - [19-47](#19-47)
  - [19-48](#19-48)
  - [19-49](#19-49)
  - [19-50](#19-50)
- [19.11 직접 상속](#1911-직접-상속)
  - [19.11.1 Object.create에 의한 직접 상속](#19111-objectcreate에-의한-직접-상속)
    - [19-51](#19-51)
    - [19-52](#19-52)
    - [19-53](#19-53)
    - [19-54](#19-54)
  - [19.11.2 객체 리터럴 내부에서 `__proto__`에 의한 직접 상속](#19112-객체-리터럴-내부에서-__proto__에-의한-직접-상속)
    - [19-55](#19-55)
  - [19.12 정적 프로퍼티/메서드](#1912-정적-프로퍼티메서드)
    - [19-56](#19-56)
    - [19-57](#19-57)
    - [19-58](#19-58)
- [19.13 프로퍼티 존재 확인](#1913-프로퍼티-존재-확인)
  - [19.13.1 in 연산자](#19131-in-연산자)
    - [19-59](#19-59)
    - [19-60](#19-60)
    - [19-61](#19-61)
  - [19.13.2 Object.prototype.hasOwnProperty 메서드](#19132-objectprototypehasownproperty-메서드)
    - [19-62](#19-62)
    - [19-63](#19-63)
- [19.14 프로퍼티 열거](#1914-프로퍼티-열거)
  - [19.14.1 for ... in 문](#19141-for--in-문)
    - [19-64](#19-64)
    - [19-65](#19-65)
    - [19-66](#19-66)
    - [19-67](#19-67)
    - [19-68](#19-68)
    - [19-69](#19-69)
    - [19-70](#19-70)
    - [19-71](#19-71)
  - [19.14.2 Object.keys/values/entries 메서드](#19142-objectkeysvaluesentries-메서드)
    - [19-72](#19-72)
    - [19-73](#19-73)
    - [19-74](#19-74)

# 19장 프로토타입

자바스크립트 : 프로토타입 기반의 객체지향 프로그래밍 언어  
자바스크립트를 이루고 있는 거의 '모든 것'이 객체. 원시 타입 값을 제외하면 모두 객체.

클래스 : ES6에서 도입됨. 클래스도 함수. 클래스와 생성자 함수는 모두 프로토타입 기반의 인스턴스를 생성하지만 정확히 동일하게 동작하지는 않음. 보다 엄격하고, 추가 기능 제공함. 클래스가 문법적 설탕보다는 새로운 객체 생성 메커니즘으로 보는 것이 타당. => 25장 클래스 참고.

# 19.1 객체 지향 프로그래밍

: 여러 개의 독립적 단위, 즉 객체의 집함으로 프로그램을 표현하려는 프로그래밍 패러다임.  
실세계의 실체를 인식하는 철학적 사고를 프로그래밍에 접목하려는 시도에서 시작.  
실체는 특징이나 성질을 나타내는 `속성`이 있고, 이를 통해 실체를 인식하거나 구분함.

추상화(abstraction) : 다양한 속성 중에서 프로그램에 필요한 속성만 간추려 내어 표현하는 것

### 19-01

객체 : 속성을 통해 여러 개의 값을 하나의 단위로 구성한 복합적인 자료구조
객체지향 프로그래밍 : 독립적인 객체의 집합으로 프로그램을 표현하려는 프로그래밍 패러다임

```javascript
// 이름과 주소 속성을 갖는 객체
const person = {
  name: "Lee",
  address: "Seoul",
};

console.log(person); // {name: "Lee", address: "Seoul"}
```

### 19-02

반지름 : 원의 '상태'를 나타내는 데이터
동작 : 원의 지름, 둘레, 넓이를 구하는 것

```javascript
const circle = {
  radius: 5, // 반지름

  // 원의 지름: 2r
  getDiameter() {
    return 2 * this.radius;
  },

  // 원의 둘레: 2πr
  getPerimeter() {
    return 2 * Math.PI * this.radius;
  },

  // 원의 넓이: πrr
  getArea() {
    return Math.PI * this.radius ** 2;
  },
};

console.log(circle);
// {radius: 5, getDiameter: ƒ, getPerimeter: ƒ, getArea: ƒ}

console.log(circle.getDiameter()); // 10
console.log(circle.getPerimeter()); // 31.41592653589793
console.log(circle.getArea()); // 78.53981633974483
```

- 상태(state) : 데이터 => `프로퍼티(property)`
- 동작(behavior) : 상태 데이터를 조작 => `메서드(method)`
- => 객체는 상태 데이터와 동작을 하나의 논리적인 단위로 묶은 복합적인 자료구조

각 객체는 고유의 기능을 갖는 독립적인 부품이자 다른 객체와 관계성을 가질 수도 있음.

# 19.2 상속과 프로토타입

상속 : 객체지향 프로그래밍의 핵심 개념, 어떤 객체의 프로퍼티 또는 메서드를 다른 객체가 상속받아 그대로 사용할 수 있는 것  
=> 자바스크립트는 프로토타입을 기반으로 상속을 구현해서 불필요한 중복 제거(중복 제거 방법 : 기존 코드 적극적 재사용)

### 19-03

인스턴스 생성할 때마다 메서드 중복 생성, 모든 인스턴스가 중복 소유  
=> 메모리 낭비, 퍼포먼스 악영향

```javascript
// 생성자 함수
function Circle(radius) {
  this.radius = radius;
  this.getArea = function () {
    // Math.PI는 원주율을 나타내는 상수다.
    return Math.PI * this.radius ** 2;
  };
}

// 반지름이 1인 인스턴스 생성
const circle1 = new Circle(1);
// 반지름이 2인 인스턴스 생성
const circle2 = new Circle(2);

// Circle 생성자 함수는 인스턴스를 생성할 때마다 동일한 동작을 하는
// getArea 메서드를 중복 생성하고 모든 인스턴스가 중복 소유한다.
// getArea 메서드는 하나만 생성하여 모든 인스턴스가 공유해서 사용하는 것이 바람직하다.
console.log(circle1.getArea === circle2.getArea); // false

console.log(circle1.getArea()); // 3.141592653589793
console.log(circle2.getArea()); // 12.566370614359172
```

### 19-04

프로토타입을 기반으로 상속 구현

```javascript
// 생성자 함수
function Circle(radius) {
  this.radius = radius;
}

// Circle 생성자 함수가 생성한 모든 인스턴스가 getArea 메서드를
// 공유해서 사용할 수 있도록 프로토타입에 추가한다.
// 프로토타입은 Circle 생성자 함수의 prototype 프로퍼티에 바인딩되어 있다.
Circle.prototype.getArea = function () {
  return Math.PI * this.radius ** 2;
};

// 인스턴스 생성
const circle1 = new Circle(1);
const circle2 = new Circle(2);

// Circle 생성자 함수가 생성한 모든 인스턴스는 부모 객체의 역할을 하는
// 프로토타입 Circle.prototype으로부터 getArea 메서드를 상속받는다.
// 즉, Circle 생성자 함수가 생성하는 모든 인스턴스는 하나의 getArea 메서드를 공유한다.
console.log(circle1.getArea === circle2.getArea); // true

console.log(circle1.getArea()); // 3.141592653589793
console.log(circle2.getArea()); // 12.566370614359172
```

상속은 코드의 재사용에서 매우 유용. 생성자 함수가 생성할 모든 인스턴스가 공통적으로 사용할 프로퍼티나 메서드를 프로토타입에 미리 구현해 두면 생성자 함수가 생성할 모든 인스턴스는 별도의 구현 없이 상위 객체인 프로토타입의 자산을 공유하여 사용할 수 있다.

# 19.3 프로토타입 객체

: 객체지향 프로그래밍의 근간을 이루는 객체 간 상속을 구현하기 위해 상속됨.

프로토타입을 상속받은 하위 객체는 상위 객체의 프로퍼티를 자신의 프로퍼티처럼 자유롭게 사용할 수 있음.

모든 객체는 [[prototype]]이라는 내부 슬롯을 가짐. 이 내부 슬롯의 값은 프로토타입의 참조. 저장되는 프로토타입은 객체 생성 방식에 의해 결정됨.

예) 객체 리터럴로 생성된 객체의 프로토타입은 Object.prototype.  
생성자 함수로 생성된 객체의 프로토타입은 생성자 함수의 prototype 프로퍼티에 바인딩되어 있는 객체.

모든 객체는 하나의 프로토타입을 가짐. 모든 프로토타입은 생성자 함수와 연결되어 있음.

[[prototype]] 내부 슬롯에서 직접 접근 불가. `__proto__` 접근자 프로퍼티로 자신의 [[Prototype]] 내부 슬롯이 가리키는 프로토타입에 간접 접근할 수 있음.

프로토타입은 자신의 constructor 프로퍼티를 통해 생성자 함수에 접근 가능.  
생성자 함수는 자신의 prototype 프로퍼티를 통해 프로토타입에 접근 가능.

## 19.3.1 `__proto__` 접근자 프로퍼티

모든 객체는 `__proto__` 접근자 프로퍼티를 통해 자신의 프로토타입, 즉 [[prototype]] 내부 슬롯에 간접 접근할 수 있음.

### 19-05

```javascript
const person = { name: "Lee" };
```

**`__proto__`는 접근자 프로퍼티다.**

내부 슬롯은 프로퍼티가 아니므로 접근, 호출할 수 있는 방법을 제공하지 않음.  
`__proto__` 접근자 프로퍼티로 간접 접근할 수 있는 것.

접근자 프로퍼티 : 자체적으로 값을 갖지 않고, [[Get]], [[Set]] 프로퍼티 어트리뷰트(다른 데이터 프로퍼티 값을 읽거나 저장할 때 사용)로 구성된 프로퍼티.

### 19-06

```javascript
const obj = {};
const parent = { x: 1 };

// getter 함수인 get __proto__가 호출되어 obj 객체의 프로토타입을 취득
obj.__proto__;
// setter함수인 set __proto__가 호출되어 obj 객체의 프로토타입을 교체
obj.__proto__ = parent;

console.log(obj.x); // 1
```

**`__proto__` 접근자 프로퍼티는 상속을 통해 사용된다.**

`__proto__` 접근자 프로퍼티는 객체가 직접 소유하는 프로퍼티가 아니라 Object.prototype의 프로퍼티임. 모든 객체는 상속을 통해 Object.prototype.`__proto__` 접근자 프로퍼티를 사용할 수 있음.

### 19-07

```javascript
const person = { name: "Lee" };

// person 객체는 __proto__ 프로퍼티를 소유하지 않는다.
console.log(person.hasOwnProperty("__proto__")); // false

// __proto__ 프로퍼티는 모든 객체의 프로토타입 객체인 Object.prototype의 접근자 프로퍼티다.
console.log(Object.getOwnPropertyDescriptor(Object.prototype, "__proto__"));
// {get: ƒ, set: ƒ, enumerable: false, configurable: true}

// 모든 객체는 Object.prototype의 접근자 프로퍼티 __proto__를 상속받아 사용할 수 있다.
console.log({}.__proto__ === Object.prototype); // true
```

프로토타입 체인의 종점, 즉 프로토타입 체인의 최상위 객체는 Object.prototype. 이 객체의 프로퍼티와 메서드는 모든 객체에 상속됨 => 19.7 프로토타입 체인 참조

**`__proto__` 접근자 프로퍼티를 통해 프로토타입에 접근하는 이유**

상호 참조에 의해 프로토타입 체인이 생성되는 것을 방지하기 위해서.

### 19-08

프로토타입 체인은 단방향 링크드 리스트. 한쪽 방향으로만 흘러가야 하고 순환 참조하는 프로토타입 체인이 만들어지면 무한 루프에 빠짐.

```javascript
const parent = {};
const child = {};

// child의 프로토타입을 parent로 설정
child.__proto__ = parent;
// parent의 프로토타입을 child로 설정
parent.__proto__ = child; // TypeError: Cyclic __proto__ value
```

**`__proto__` 접근자 프로퍼티를 코드 내에서 직접 사용하는 것은 권장하지 않는다.**

모든 객체가 `__proto__` 접근자 프로퍼티를 사용할 수 있는 것은 아니기 때문.

### 19-09

```javascript
// obj는 프로토타입 체인의 종점이다. 따라서 Object.__proto__를 상속받을 수 없다.
const obj = Object.create(null);

// obj는 Object.__proto__를 상속받을 수 없다.
console.log(obj.__proto__); // undefined

// 따라서 __proto__보다 Object.getPrototypeOf 메서드를 사용하는 편이 좋다.
console.log(Object.getPrototypeOf(obj)); // null
```

### 19-10

프로토타입의 참조를 취득하고 싶은 경우에는 Object.getPrototypeOf 메서드 사용
프로토타입을 교체하고 싶은 경우에는 Object.setPrototypeOf 메서드 사용 권장
=> `__proto__`으로 처리 내용과 정확히 일치

```javascript
const obj = {};
const parent = { x: 1 };

// obj 객체의 프로토타입을 취득
Object.getPrototypeOf(obj); // obj.__proto__;
// obj 객체의 프로토타입을 교체
Object.setPrototypeOf(obj, parent); // obj.__proto__ = parent;

console.log(obj.x); // 1
```

## 19.3.2 함수 객체의 prototype 프로퍼티

함수 객체만이 소유하는 prototype 프로퍼티는 생성자 함수가 생성할 인스턴스의 프로토타입 가리킴.

### 19-11

```javascript
// 함수 객체는 prototype 프로퍼티를 소유한다.
(function () {}).hasOwnProperty("prototype"); // -> true

// 일반 객체는 prototype 프로퍼티를 소유하지 않는다.
({}).hasOwnProperty("prototype"); // -> false
```

### 19-12

non-constructor인 화살표 함수와 메서드는 prototype 프로퍼티를 소유하지 않으며 프로토타입도 생성하지 않음.

```javascript
// 화살표 함수는 non-constructor다.
const Person = (name) => {
  this.name = name;
};

// non-constructor는 prototype 프로퍼티를 소유하지 않는다.
console.log(Person.hasOwnProperty("prototype")); // false

// non-constructor는 프로토타입을 생성하지 않는다.
console.log(Person.prototype); // undefined

// ES6의 메서드 축약 표현으로 정의한 메서드는 non-constructor다.
const obj = {
  foo() {},
};

// non-constructor는 prototype 프로퍼티를 소유하지 않는다.
console.log(obj.foo.hasOwnProperty("prototype")); // false

// non-constructor는 프로토타입을 생성하지 않는다.
console.log(obj.foo.prototype); // undefined
```

생성자 함수로 사용된 것이 아닌  
일반 함수(함수 선언문, 함수 표현식)는 prototype 프로퍼티를 소유하지만 객체를 생성하지 않는 일반 함수의 prototype 프로퍼티는 아무 의미가 없음.

모든 객체가 가지고 있는 `__proto__` 접근자 프로퍼티  
함수 객체만이 가지고 있는 prototype 프로퍼티  
=> 동일한 프로토타입 가리킴

- `__proto__` 접근자 프로퍼티

  - 모든 객체가 가지고 있음
  - 객체가 자신의 프로토타입에 접근 또는 교체하기 위해 사용

- prototype 프로퍼티
  - 함수가 가지고 있음
  - 생성자 함수가 자신이 생설할 객체(인스턴스)의 프로토타입을 할당하기 위해 사용

### 19-13

```javascript
// 생성자 함수
function Person(name) {
  this.name = name;
}

const me = new Person("Lee");

// 결국 Person.prototype과 me.__proto__는 결국 동일한 프로토타입을 가리킨다.
console.log(Person.prototype === me.__proto__); // true
```

## 19.3.3 프로토타입의 constructor 프로퍼티와 생성자 함수

모든 프로토타입은 constructor 프로퍼티를 가짐. 이 constructor 프로퍼티는 prototype 프로퍼티로 자신을 참조하고 있는 생성자 함수를 가리킨다.  
생성자 함수가 생성될 때(함수 객체가 생성될 때) `연결`됨

### 19-14

Person 생성자 함수 => me 객체 생성.  
me 객체는 프로토타입의 constructor 프로퍼티를 통해 생성자 함수와 연결됨.  
me 객체에는 constructor 프로퍼티가 없음.  
me 객체의 프로토타입인 Person.prototype에 constructor 프로퍼티가 있음.  
me 객체는 프로토타입인 Person.prototype의 constructor 프로퍼티를 상속받아 사용할 수 있음.

```javascript
// 생성자 함수
function Person(name) {
  this.name = name;
}

const me = new Person("Lee");

// me 객체의 생성자 함수는 Person이다.
console.log(me.constructor === Person); // true
```

# 19.4 리터럴 표기법에 의해 생성된 객체의 생성자 함수와 프로토타입

생성자 함수에 의해 생성된 인스턴스는  
프로토타입의 constructor 프로퍼티에 의해 생성자 함수와 연결됨.  
이때 constructor 프로퍼티가 가리키는 생성자 함수는 인스턴스를 생성한 생성자 함수다.

### 19-15

```javascript
// obj 객체를 생성한 생성자 함수는 Object다.
const obj = new Object();
console.log(obj.constructor === Object); // true

// add 함수 객체를 생성한 생성자 함수는 Function이다.
const add = new Function("a", "b", "return a + b");
console.log(add.constructor === Function); // true

// 생성자 함수
function Person(name) {
  this.name = name;
}

// me 객체를 생성한 생성자 함수는 Person이다.
const me = new Person("Lee");
console.log(me.constructor === Person); // true
```

### 19-16

인스턴스를 생성하지 않는 객체 생성 방식  
(리터럴 표기법)

```javascript
// 객체 리터럴
const obj = {};

// 함수 리터럴
const add = function (a, b) {
  return a + b;
};

// 배열 리터럴
const arr = [1, 2, 3];

// 정규표현식 리터럴
const regexp = /is/gi;
```

리터럴 표기법에 의해 생성된 객체도 프로토타입이 존재하지만  
프로토타입의 constructor 프로퍼티가 가리키는 생성자 함수가  
반드시 객체를 생성한 생성자 함수라고 단정할 수 없음.

### 19-17

```javascript
// obj 객체는 Object 생성자 함수로 생성한 객체가 아니라 객체 리터럴로 생성했다.
const obj = {};

// 하지만 obj 객체의 생성자 함수는 Object 생성자 함수다.
console.log(obj.constructor === Object); // true
```

### 19-18

```javascript
// 2. Object 생성자 함수에 의한 객체 생성
// 인수가 전달되지 않았을 때 추상 연산 OrdinaryObjectCreate를 호출하여 빈 객체를 생성한다.
let obj = new Object();
console.log(obj); // {}

// 1. new.target이 undefined나 Object가 아닌 경우
// 인스턴스 -> Foo.prototype -> Object.prototype 순으로 프로토타입 체인이 생성된다.
class Foo extends Object {}
new Foo(); // Foo {}

// 3. 인수가 전달된 경우에는 인수를 객체로 변환한다.
// Number 객체 생성
obj = new Object(123);
console.log(obj); // Number {123}

// String  객체 생성
obj = new Object("123");
console.log(obj); // String {"123"}
```

Object 생성자 함수 호출과  
객체 리터럴의 평가  
공통점 : 추상 연산 OrdinaryObjectCreate를 호출하여 빈 객체를 생성  
차이점 : new.target 확인, 프로퍼티를 추가하는 처리  
=> 객체 리터럴에 의해 생성된 객체는 Object 생성자 함수가 생성한 객체가 아님.

### 19-19

```javascript
// foo 함수는 Function 생성자 함수로 생성한 함수 객체가 아니라 함수 선언문으로 생성했다.
function foo() {}

// 하지만 constructor 프로퍼티를 통해 확인해보면 함수 foo의 생성자 함수는 Function 생성자 함수다.
console.log(foo.constructor === Function); // true
```

리터럴 표기법에 의해 생성된 객체도 상속을 위해 프로토타입이 필요하고, 가상적인 생성자 함수를 가짐.  
프로토타입은 생성자 함수와 더불어 생성되며, prototype, constructor 프로퍼티에 의해 연결되어 있기 때문.  
프로토타입과 생성자 함수는 단독으로 존재할 수 없고, 언제나 쌍(pair)으로 존재함.

리터럴 표기법에 의해 생성된 객체는  
생성자 함수에 의해 생성된 객체가 아님.  
그러나 본질적인 면에서 큰 차이가 없음.

프로토타입의 constructor 프로퍼티를 통해 연결되어 있는 생성자 함수를  
리터럴 표기법으로 생성한 객체를 생성한 생성자 함수로 생각해도  
크게 무리 없음.

|   리터럴 표기법    | 생성자 함수 |     프로토타입     |
| :----------------: | :---------: | :----------------: |
|    객체 리터럴     |   Object    |  Object.prototype  |
|    함수 리터럴     |  Function   | Function.prototype |
|    배열 리터럴     |    Array    |  Array.prototype   |
| 정규 표현식 리터럴 |   RegExp    |  RegExp.prototype  |

=> 리터럴 표기법에 의해 생성된 객체의 생성자 함수와 프로토타입

# 19.5 프로토타입 생성 시점

`모든 객체는 생성자 함수와 연결되어 있다.`  
`프로토타입은 생성자 함수가 생성되는 시점에 더불어 생성된다.`  
(프로토타입과 생성자 함수는 언제나 쌍으로 존재)

- 생성자 함수
  - 사용자가 직접 정의한 사용자 정의 생성자 함수
  - 자바스크립트가 기본 제공하는 빌트인 생성자 함수

## 19.5.1 사용자 정의 생성자 함수와 프로토타입 생성 시점

일반 함수(함수 선언문, 함수 표현식)로 정의한 함수 객체는 new 연산자와 함께 생성자 함수로서 호출할 수 있음.

생성자 함수로서 호출할 수 있는 함수, 즉 constructor는 함수 정의가 평가되어 함수 객체를 생성하는 시점에 프로토타입도 더불어 생성됨.

### 19-20

```javascript
// 함수 정의(constructor)가 평가되어 함수 객체를 생성하는 시점에 프로토타입도 더불어 생성된다.
console.log(Person.prototype); // {constructor: ƒ}

// 생성자 함수
function Person(name) {
  this.name = name;
}
```

### 19-21

non-constructor는 프로토타입이 생성되지 않음.

```javascript
// 화살표 함수는 non-constructor다.
const Person = (name) => {
  this.name = name;
};

// non-constructor는 프로토타입이 생성되지 않는다.
console.log(Person.prototype); // undefined
```

함수 선언문은 런타임 이전에 자바스크립트 엔진에 의해 먼저 실행됨.  
Person 생성자 함수는 먼저 평가되어 함수 객체가 되고 프로토타입도 더불어 생성됨.  
생성된 프로토타입은 Person 생성자 함수의 prototype 프로퍼티에 바인딩됨.

생성된 프로토타입은 오직 constructor 프로퍼티만을 갖는 객체.  
프로토타입도 객체, 모든 객체는 프로토타입을 가지므로  
프로토타입도 자신의 프로토타입을 가짐.  
생성된 프로토타입의 프로토타입은 Object.prototype이다.

## 19.5.2 빌트인 생성자 함수와 프로토타입 생성 시점

빌트인 생성자 함수도 빌트인 생성자 함수가 생성되는 시점에 프로토타입이 생성됨.  
모든 빌트인 생성자 함수는 전역 객체가 생성되는 시점에 생성됨.  
생성된 프로토타입은 빌트인 생성자 함수의 prototype 프로퍼티에 바인딩됨.

### 19-22

- 전역 객체의 프로퍼티
  - 표준 빌트인 객체(Object, String, Number, Function, Array ...)
  - 환경에 따른 호스트 객체(클라이언트 Web API, Node.js의 호스트 API)
  - var 키워드로 선언한 전역 변수와 전역 함수

```javascript
// 전역 객체 window는 브라우저에 종속적이므로 아래 코드는 브라우저 환경에서 실행해야 한다.
// 빌트인 객체인 Object는 전역 객체 window의 프로퍼티다.
window.Object === Object; // true
```

객체가 생성되기 이전에 생성자 함수와 프로토타입은 이미 객체화되어 존재함.  
이후 생성자 함수 또는 리터럴 표기법으로 객체를 생성하면 프로토타입은 생성된 객체의 [[Prototype]] 내부 슬롯에 할당된다.  
이로써 생성된 객체는 프로토타입을 상속받는다.

# 19.6 객체 생성 방식과 프로토타입의 결정

- 객체 생성 방법
  - 객체 리터럴
  - Object 생성자 함수
  - 생성자 함수
  - Object.create 메서드
  - 클래스(ES6)

세부적인 객체 생성 방식 차이가 있지만, 추상 연산 OrdinaryObjectCreate에 의해 생성된다는 공통점이 있음

추상 연산 OrdinaryObjectCreate는  
필수적으로 자신이 생성할 객체의 프로토타입을 인수로 전달받음.  
그리고 자신이 생성할 `객체에 추가할 프로퍼티 목록`을 옵션으로 전달할 수 있음.  
추상 연산 OrdinaryObjectCreate는 빈 객체를 생성한 후, `객체에 추가할 프로퍼티 목록`이 전달된 경우 프로퍼티를 객체에 추가함.  
인수로 전달받은 프로토타입을 자신이 생성한 객체의 [[Prototype]] 내부 슬롯에 할당한 다음, 생성한 객체를 반환함.

프로토타입은 추상 연산 OrdinaryObjectCreate에 전달되는 인수에 의해 결정됨.  
이 인수는 객체가 생성되는 시점에 객체 생성 방식에 의해 결정됨.

## 19.6.1 객체 리터럴에 의해 생성된 객체의 프로토타입

객체를 생성할 때 추상 연산 OrdinaryObjectCreate를 호출함.

### 19-23

```javascript
const obj = { x: 1 };
```

### 19-24

```javascript
const obj = { x: 1 };

// 객체 리터럴에 의해 생성된 obj 객체는 Object.prototype을 상속받는다.
console.log(obj.constructor === Object); // true
console.log(obj.hasOwnProperty("x")); // true
```

## 19.6.2 Object 생성자 함수에 의해 생성된 객체의 프로토타입

### 19-25

```javascript
const obj = new Object();
obj.x = 1;
```

### 19-26

```javascript
const obj = new Object();
obj.x = 1;

// Object 생성자 함수에 의해 생성된 obj 객체는 Object.prototype을 상속받는다.
console.log(obj.constructor === Object); // true
console.log(obj.hasOwnProperty("x")); // true
```

## 19.6.3 생성자 함수에 의해 생성된 객체의 프로토타입

### 19-27

```javascript
function Person(name) {
  this.name = name;
}

const me = new Person("Lee");
```

### 19-28

```javascript
function Person(name) {
  this.name = name;
}

// 프로토타입 메서드
Person.prototype.sayHello = function () {
  console.log(`Hi! My name is ${this.name}`);
};

const me = new Person("Lee");
const you = new Person("Kim");

me.sayHello(); // Hi! My name is Lee
you.sayHello(); // Hi! My name is Kim
```

# 19.7 프로토타입 체인

### 19-29

```javascript
function Person(name) {
  this.name = name;
}

// 프로토타입 메서드
Person.prototype.sayHello = function () {
  console.log(`Hi! My name is ${this.name}`);
};

const me = new Person("Lee");

// hasOwnProperty는 Object.prototype의 메서드다.
console.log(me.hasOwnProperty("name")); // true
```

### 19-30

```javascript
Object.getPrototypeOf(me) === Person.prototype; // -> true
```

### 19-31

```javascript
Object.getPrototypeOf(Person.prototype) === Object.prototype; // -> true
```

### 19-32

```javascript
// hasOwnProperty는 Object.prototype의 메서드다.
// me 객체는 프로토타입 체인을 따라 hasOwnProperty 메서드를 검색하여 사용한다.
me.hasOwnProperty("name"); // -> true
```

### 19-33

```javascript
Object.prototype.hasOwnProperty.call(me, "name");
```

### 19-34

```javascript
console.log(me.foo); // undefined
```

### 19-35

```javascript
me.hasOwnProperty("name");
```

# 19.8 오버라이딩과 프로퍼티 섀도잉

### 19-36

```javascript
const Person = (function () {
  // 생성자 함수
  function Person(name) {
    this.name = name;
  }

  // 프로토타입 메서드
  Person.prototype.sayHello = function () {
    console.log(`Hi! My name is ${this.name}`);
  };

  // 생성자 함수를 반환
  return Person;
})();

const me = new Person("Lee");

// 인스턴스 메서드
me.sayHello = function () {
  console.log(`Hey! My name is ${this.name}`);
};

// 인스턴스 메서드가 호출된다. 프로토타입 메서드는 인스턴스 메서드에 의해 가려진다.
me.sayHello(); // Hey! My name is Lee
```

### 19-37

```javascript
// 인스턴스 메서드를 삭제한다.
delete me.sayHello;
// 인스턴스에는 sayHello 메서드가 없으므로 프로토타입 메서드가 호출된다.
me.sayHello(); // Hi! My name is Lee
```

### 19-38

```javascript
// 프로토타입 체인을 통해 프로토타입 메서드가 삭제되지 않는다.
delete me.sayHello;
// 프로토타입 메서드가 호출된다.
me.sayHello(); // Hi! My name is Lee
```

### 19-39

```javascript
// 프로토타입 메서드 변경
Person.prototype.sayHello = function () {
  console.log(`Hey! My name is ${this.name}`);
};
me.sayHello(); // Hey! My name is Lee

// 프로토타입 메서드 삭제
delete Person.prototype.sayHello;
me.sayHello(); // TypeError: me.sayHello is not a function
```

# 19.9 프로토타입의 교체

## 19.9.1 생성자 함수에 의한 프로토타입의 교체

### 19-40

```javascript
const Person = (function () {
  function Person(name) {
    this.name = name;
  }

  // ① 생성자 함수의 prototype 프로퍼티를 통해 프로토타입을 교체
  Person.prototype = {
    sayHello() {
      console.log(`Hi! My name is ${this.name}`);
    },
  };

  return Person;
})();

const me = new Person("Lee");
```

### 19-41

```javascript
// 프로토타입을 교체하면 constructor 프로퍼티와 생성자 함수 간의 연결이 파괴된다.
console.log(me.constructor === Person); // false
// 프로토타입 체인을 따라 Object.prototype의 constructor 프로퍼티가 검색된다.
console.log(me.constructor === Object); // true
```

### 19-42

```javascript
const Person = (function () {
  function Person(name) {
    this.name = name;
  }

  // 생성자 함수의 prototype 프로퍼티를 통해 프로토타입을 교체
  Person.prototype = {
    // constructor 프로퍼티와 생성자 함수 간의 연결을 설정
    constructor: Person,
    sayHello() {
      console.log(`Hi! My name is ${this.name}`);
    },
  };

  return Person;
})();

const me = new Person("Lee");

// constructor 프로퍼티가 생성자 함수를 가리킨다.
console.log(me.constructor === Person); // true
console.log(me.constructor === Object); // false
```

## 19.9.2 인스턴스에 의한 프로토타입의 교체

### 19-43

```javascript
function Person(name) {
  this.name = name;
}

const me = new Person("Lee");

// 프로토타입으로 교체할 객체
const parent = {
  sayHello() {
    console.log(`Hi! My name is ${this.name}`);
  },
};

// ① me 객체의 프로토타입을 parent 객체로 교체한다.
Object.setPrototypeOf(me, parent);
// 위 코드는 아래의 코드와 동일하게 동작한다.
// me.__proto__ = parent;

me.sayHello(); // Hi! My name is Lee
```

### 19-44

```javascript
// 프로토타입을 교체하면 constructor 프로퍼티와 생성자 함수 간의 연결이 파괴된다.
console.log(me.constructor === Person); // false
// 프로토타입 체인을 따라 Object.prototype의 constructor 프로퍼티가 검색된다.
console.log(me.constructor === Object); // true
```

### 19-45

```javascript
function Person(name) {
  this.name = name;
}

const me = new Person("Lee");

// 프로토타입으로 교체할 객체
const parent = {
  // constructor 프로퍼티와 생성자 함수 간의 연결을 설정
  constructor: Person,
  sayHello() {
    console.log(`Hi! My name is ${this.name}`);
  },
};

// 생성자 함수의 prototype 프로퍼티와 프로토타입 간의 연결을 설정
Person.prototype = parent;

// me 객체의 프로토타입을 parent 객체로 교체한다.
Object.setPrototypeOf(me, parent);
// 위 코드는 아래의 코드와 동일하게 동작한다.
// me.__proto__ = parent;

me.sayHello(); // Hi! My name is Lee

// constructor 프로퍼티가 생성자 함수를 가리킨다.
console.log(me.constructor === Person); // true
console.log(me.constructor === Object); // false

// 생성자 함수의 prototype 프로퍼티가 교체된 프로토타입을 가리킨다.
console.log(Person.prototype === Object.getPrototypeOf(me)); // true
```

# 19.10 instanceof 연산자

### 19-46

```javascript
// 생성자 함수
function Person(name) {
  this.name = name;
}

const me = new Person("Lee");

// Person.prototype이 me 객체의 프로토타입 체인 상에 존재하므로 true로 평가된다.
console.log(me instanceof Person); // true

// Object.prototype이 me 객체의 프로토타입 체인 상에 존재하므로 true로 평가된다.
console.log(me instanceof Object); // true
```

### 19-47

```javascript
// 생성자 함수
function Person(name) {
  this.name = name;
}

const me = new Person("Lee");

// 프로토타입으로 교체할 객체
const parent = {};

// 프로토타입의 교체
Object.setPrototypeOf(me, parent);

// Person 생성자 함수와 parent 객체는 연결되어 있지 않다.
console.log(Person.prototype === parent); // false
console.log(parent.constructor === Person); // false

// Person.prototype이 me 객체의 프로토타입 체인 상에 존재하지 않기 때문에 false로 평가된다.
console.log(me instanceof Person); // false

// Object.prototype이 me 객체의 프로토타입 체인 상에 존재하므로 true로 평가된다.
console.log(me instanceof Object); // true
```

### 19-48

```javascript
// 생성자 함수
function Person(name) {
  this.name = name;
}

const me = new Person("Lee");

// 프로토타입으로 교체할 객체
const parent = {};

// 프로토타입의 교체
Object.setPrototypeOf(me, parent);

// Person 생성자 함수와 parent 객체는 연결되어 있지 않다.
console.log(Person.prototype === parent); // false
console.log(parent.constructor === Person); // false

// parent 객체를 Person 생성자 함수의 prototype 프로퍼티에 바인딩한다.
Person.prototype = parent;

// Person.prototype이 me 객체의 프로토타입 체인 상에 존재하므로 true로 평가된다.
console.log(me instanceof Person); // true

// Object.prototype이 me 객체의 프로토타입 체인 상에 존재하므로 true로 평가된다.
console.log(me instanceof Object); // true
```

### 19-49

```javascript
function isInstanceof(instance, constructor) {
  // 프로토타입 취득
  const prototype = Object.getPrototypeOf(instance);

  // 재귀 탈출 조건
  // prototype이 null이면 프로토타입 체인의 종점에 다다른 것이다.
  if (prototype === null) return false;

  // 프로토타입이 생성자 함수의 prototype 프로퍼티에 바인딩된 객체라면 true를 반환한다.
  // 그렇지 않다면 재귀 호출로 프로토타입 체인 상의 상위 프로토타입으로 이동하여 확인한다.
  return (
    prototype === constructor.prototype || isInstanceof(prototype, constructor)
  );
}

console.log(isInstanceof(me, Person)); // true
console.log(isInstanceof(me, Object)); // true
console.log(isInstanceof(me, Array)); // false
```

### 19-50

```javascript
const Person = (function () {
  function Person(name) {
    this.name = name;
  }

  // 생성자 함수의 prototype 프로퍼티를 통해 프로토타입을 교체
  Person.prototype = {
    sayHello() {
      console.log(`Hi! My name is ${this.name}`);
    },
  };

  return Person;
})();

const me = new Person("Lee");

// constructor 프로퍼티와 생성자 함수 간의 연결은 파괴되어도 instanceof는 아무런 영향을 받지 않는다.
console.log(me.constructor === Person); // false

// Person.prototype이 me 객체의 프로토타입 체인 상에 존재하므로 true로 평가된다.
console.log(me instanceof Person); // true
// Object.prototype이 me 객체의 프로토타입 체인 상에 존재하므로 true로 평가된다.
console.log(me instanceof Object); // true
```

# 19.11 직접 상속

## 19.11.1 Object.create에 의한 직접 상속

### 19-51

```javascript
// 프로토타입이 null인 객체를 생성한다. 생성된 객체는 프로토타입 체인의 종점에 위치한다.
// obj → null
let obj = Object.create(null);
console.log(Object.getPrototypeOf(obj) === null); // true
// Object.prototype을 상속받지 못한다.
console.log(obj.toString()); // TypeError: obj.toString is not a function

// obj → Object.prototype → null
// obj = {};와 동일하다.
obj = Object.create(Object.prototype);
console.log(Object.getPrototypeOf(obj) === Object.prototype); // true

// obj → Object.prototype → null
// obj = { x: 1 };와 동일하다.
obj = Object.create(Object.prototype, {
  x: { value: 1, writable: true, enumerable: true, configurable: true },
});
// 위 코드는 다음과 동일하다.
// obj = Object.create(Object.prototype);
// obj.x = 1;
console.log(obj.x); // 1
console.log(Object.getPrototypeOf(obj) === Object.prototype); // true

const myProto = { x: 10 };
// 임의의 객체를 직접 상속받는다.
// obj → myProto → Object.prototype → null
obj = Object.create(myProto);
console.log(obj.x); // 10
console.log(Object.getPrototypeOf(obj) === myProto); // true

// 생성자 함수
function Person(name) {
  this.name = name;
}

// obj → Person.prototype → Object.prototype → null
// obj = new Person('Lee')와 동일하다.
obj = Object.create(Person.prototype);
obj.name = "Lee";
console.log(obj.name); // Lee
console.log(Object.getPrototypeOf(obj) === Person.prototype); // true
```

### 19-52

```javascript
const obj = { a: 1 };

obj.hasOwnProperty("a"); // -> true
obj.propertyIsEnumerable("a"); // -> true
```

### 19-53

```javascript
// 프로토타입이 null인 객체, 즉 프로토타입 체인의 종점에 위치하는 객체를 생성한다.
const obj = Object.create(null);
obj.a = 1;

console.log(Object.getPrototypeOf(obj) === null); // true

// obj는 Object.prototype의 빌트인 메서드를 사용할 수 없다.
console.log(obj.hasOwnProperty("a")); // TypeError: obj.hasOwnProperty is not a function
```

### 19-54

```javascript
// 프로토타입이 null인 객체를 생성한다.
const obj = Object.create(null);
obj.a = 1;

// console.log(obj.hasOwnProperty('a')); // TypeError: obj.hasOwnProperty is not a function

// Object.prototype의 빌트인 메서드는 객체로 직접 호출하지 않는다.
console.log(Object.prototype.hasOwnProperty.call(obj, "a")); // true
```

## 19.11.2 객체 리터럴 내부에서 `__proto__`에 의한 직접 상속

### 19-55

```javascript
const myProto = { x: 10 };

// 객체 리터럴에 의해 객체를 생성하면서 프로토타입을 지정하여 직접 상속받을 수 있다.
const obj = {
  y: 20,
  // 객체를 직접 상속받는다.
  // obj → myProto → Object.prototype → null
  __proto__: myProto,
};
/* 위 코드는 아래와 동일하다.
const obj = Object.create(myProto, {
  y: { value: 20, writable: true, enumerable: true, configurable: true }
});
*/

console.log(obj.x, obj.y); // 10 20
console.log(Object.getPrototypeOf(obj) === myProto); // true
```

## 19.12 정적 프로퍼티/메서드

### 19-56

```javascript
// 생성자 함수
function Person(name) {
  this.name = name;
}

// 프로토타입 메서드
Person.prototype.sayHello = function () {
  console.log(`Hi! My name is ${this.name}`);
};

// 정적 프로퍼티
Person.staticProp = "static prop";

// 정적 메서드
Person.staticMethod = function () {
  console.log("staticMethod");
};

const me = new Person("Lee");

// 생성자 함수에 추가한 정적 프로퍼티/메서드는 생성자 함수로 참조/호출한다.
Person.staticMethod(); // staticMethod

// 정적 프로퍼티/메서드는 생성자 함수가 생성한 인스턴스로 참조/호출할 수 없다.
// 인스턴스로 참조/호출할 수 있는 프로퍼티/메서드는 프로토타입 체인 상에 존재해야 한다.
me.staticMethod(); // TypeError: me.staticMethod is not a function
```

### 19-57

```javascript
// Object.create는 정적 메서드다.
const obj = Object.create({ name: "Lee" });

// Object.prototype.hasOwnProperty는 프로토타입 메서드다.
obj.hasOwnProperty("name"); // -> false
```

### 19-58

```javascript
function Foo() {}

// 프로토타입 메서드
// this를 참조하지 않는 프로토타입 메소드는 정적 메서드로 변경해도 동일한 효과를 얻을 수 있다.
Foo.prototype.x = function () {
  console.log("x");
};

const foo = new Foo();
// 프로토타입 메서드를 호출하려면 인스턴스를 생성해야 한다.
foo.x(); // x

// 정적 메서드
Foo.x = function () {
  console.log("x");
};

// 정적 메서드는 인스턴스를 생성하지 않아도 호출할 수 있다.
Foo.x(); // x
```

# 19.13 프로퍼티 존재 확인

## 19.13.1 in 연산자

### 19-59

```javascript
const person = {
  name: "Lee",
  address: "Seoul",
};

// person 객체에 name 프로퍼티가 존재한다.
console.log("name" in person); // true
// person 객체에 address 프로퍼티가 존재한다.
console.log("address" in person); // true
// person 객체에 age 프로퍼티가 존재하지 않는다.
console.log("age" in person); // false
```

### 19-60

```javascript
console.log("toString" in person); // true
```

### 19-61

```javascript
const person = { name: "Lee" };

console.log(Reflect.has(person, "name")); // true
console.log(Reflect.has(person, "toString")); // true
```

## 19.13.2 Object.prototype.hasOwnProperty 메서드

### 19-62

```javascript
console.log(person.hasOwnProperty("name")); // true
console.log(person.hasOwnProperty("age")); // false
```

### 19-63

```javascript
console.log(person.hasOwnProperty("toString")); // false
```

# 19.14 프로퍼티 열거

## 19.14.1 for ... in 문

### 19-64

```javascript
const person = {
  name: "Lee",
  address: "Seoul",
};

// for...in 문의 변수 key에 person 객체의 프로퍼티 키가 할당된다.
for (const key in person) {
  console.log(key + ": " + person[key]);
}
// name: Lee
// address: Seoul
```

### 19-65

```javascript
const person = {
  name: "Lee",
  address: "Seoul",
};

// in 연산자는 객체가 상속받은 모든 프로토타입의 프로퍼티를 확인한다.
console.log("toString" in person); // true

// for...in 문도 객체가 상속받은 모든 프로토타입의 프로퍼티를 열거한다.
// 하지만 toString과 같은 Object.prototype의 프로퍼티가 열거되지 않는다.
for (const key in person) {
  console.log(key + ": " + person[key]);
}

// name: Lee
// address: Seoul
```

### 19-66

```javascript
// Object.getOwnPropertyDescriptor 메서드는 프로퍼티 디스크립터 객체를 반환한다.
// 프로퍼티 디스크립터 객체는 프로퍼티 어트리뷰트 정보를 담고 있는 객체다.
console.log(Object.getOwnPropertyDescriptor(Object.prototype, "toString"));
// {value: ƒ, writable: true, enumerable: false, configurable: true}
```

### 19-67

```javascript
const person = {
  name: "Lee",
  address: "Seoul",
  __proto__: { age: 20 },
};

for (const key in person) {
  console.log(key + ": " + person[key]);
}
// name: Lee
// address: Seoul
// age: 20
```

### 19-68

```javascript
const sym = Symbol();
const obj = {
  a: 1,
  [sym]: 10,
};

for (const key in obj) {
  console.log(key + ": " + obj[key]);
}
// a: 1
```

### 19-69

```javascript
const person = {
  name: "Lee",
  address: "Seoul",
  __proto__: { age: 20 },
};

for (const key in person) {
  // 객체 자신의 프로퍼티인지 확인한다.
  if (!person.hasOwnProperty(key)) continue;
  console.log(key + ": " + person[key]);
}
// name: Lee
// address: Seoul
```

### 19-70

```javascript
const obj = {
  2: 2,
  3: 3,
  1: 1,
  b: "b",
  a: "a",
};

for (const key in obj) {
  if (!obj.hasOwnProperty(key)) continue;
  console.log(key + ": " + obj[key]);
}

/*
1: 1
2: 2
3: 3
b: b
a: a
*/
```

### 19-71

```javascript
const arr = [1, 2, 3];
arr.x = 10; // 배열도 객체이므로 프로퍼티를 가질 수 있다.

for (const i in arr) {
  // 프로퍼티 x도 출력된다.
  console.log(arr[i]); // 1 2 3 10
}

// arr.length는 3이다.
for (let i = 0; i < arr.length; i++) {
  console.log(arr[i]); // 1 2 3
}

// forEach 메서드는 요소가 아닌 프로퍼티는 제외한다.
arr.forEach((v) => console.log(v)); // 1 2 3

// for...of는 변수 선언문에서 선언한 변수에 키가 아닌 값을 할당한다.
for (const value of arr) {
  console.log(value); // 1 2 3
}
```

## 19.14.2 Object.keys/values/entries 메서드

### 19-72

```javascript
const person = {
  name: "Lee",
  address: "Seoul",
  __proto__: { age: 20 },
};

console.log(Object.keys(person)); // ["name", "address"]
```

### 19-73

```javascript
console.log(Object.values(person)); // ["Lee", "Seoul"]
```

### 19-74

```javascript
console.log(Object.entries(person)); // [["name", "Lee"], ["address", "Seoul"]]

Object.entries(person).forEach(([key, value]) => console.log(key, value));
/*
name Lee
address Seoul
*/
```