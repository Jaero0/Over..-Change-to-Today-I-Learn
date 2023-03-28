# 일일회고

## 목적
배우고 직접 적어보지 않으면 까먹는다   
그러므로 노트든 블로그든 어디든 배운 내용을 적어가며 암기한다   
그래서 난 깃허브 daily commit을 선택했다   
복습! 반복!

## 개인 회고 (28, 03, 2023)
토요일과 일요일의 일.. 아침 10시부터 새벽 1시까지 주말내내 일했다.. 그러고 사장은 나에게 밥사주는데 뭐가문제냐... 라는 말을했고.. <br><br>
나의 일은 거기에서 끝났다. 허리도 아프고 어제 하루종일 자기만 했다.. 오늘부턴 다시 시작이다! <br><br>
중요하다고 하는 함수파트라 확실하게 이해하고 넘어가고자 더욱 자세하게 커밋을 작성!
- - - -
# 3/28(화)

## 1. Today I learned
### 1. JavaScript 함수
#### 1. 함수는 여러동작을 묶어놓은 것이다.
  1. 자주 사용할것 같은 기능은 그 기능에 필요할것같은 동작을 함수로 묶을수있다. <br><br>
     * ex) function ???() {} <-- 한번 선언하면 그 스크립트 어디에서든지 사용할수있다! 이렇게 "함수선언" 후 함수를 다시 "함수실행" 해주어야한다. <br><br>
  2. 함수스코프 안에는 블럭스코프를 선언이 가능하지만 반대로는 불가능! 하지만.. ES6부터는 함수표현식(function)을 통해 선언이 가능... <br><br>
  3. **함수문장은 hoisting의 대상이 된다. 함수가 위치한 곳에 관계없이 유효범위의 가장 상위로 이동된다.<br>
  그렇기때문에 함수 호출이 함수를 정의하는 문장보다 앞에 있건, 뒤에 있건 유효범위만 같으면 문제가 없다.** <br><br>
  
#### 2. 여러번 사용할 수 있는 함수 만들기
  1. 매개변수와 인수! <br><br>
     * Parameter, 매개변수는 function addNum( **a, b**), 인수는 addNum( **2, 3**) <br><br>
  2. **Return** <br><br>
     * 함수 안에서 다 해결이 되면 상관없지만 함수 밖에서 함수 값을 불러와야 할때, <br><br>
     즉, 함수를 실행한 후 결괏값을 함수 밖으로 넘기는 것을 **함수값을 반환한다. RETURN** 이라함! <br><br>
     
```javascript
function addNum(a, b) { //함수 선언 #1
  let sum = a + b; #4
  return sum; //sum값을 함수 밖으로 꺼내기 위한 return사용!#5 
}

let num1 = parseInt(prompt("Insert first number")); //#2
let num2 = parseInt(prompt("Insert second number")); //#2
let result = addNum(num1, num2); //result는 addNum의 함수 a,b의 값에 num1과 num2를 넣은 값이다! #3 --> #6
```

### 2. JavaScript var, let, const와 호이스팅
  1. var let const의 scope와 scope란 무엇인지에 대해 이미 정리해놓음! <br><br>
     1. [2. Today I found out! 을 확인해보자!](https://github.com/Jaero0/DailyCommitBeginner_till_ExpertBackend/blob/main/Commits/16%2C03%2C2023.md) <br><br>
  2. var변수의 호이스팅이란? <br><br>
     1. 호이스팅은 var변수에서 값을 지정하기 전에 미리 시스템적으로 undefined값을 지정한다! 따라서 오류가 발생하지 않고 값이 선언안되면 undefined로 출력! <br><br>
  3. 함수내에서는 어떤 변수를 사용하건 (const제외) 다 함수스코프로 사용이 된다! <br><br>
 
### 3. JavaScript 함수 표현식
#### 1. 익명함수
  * 익명함수는 함수 자체가 식이기에 변수에 할당 가능!, 또 다른 함수의 매개변수로 활용가능! <br><br>

```javascript
사용예시

let add = function(a, b) { //add변수에 바로 익명함수 할당!
  return a + b; //함수 밖으로 결괏값을 이동하기 위한 반환! 
}

let sum = add(10, 20) // sum변수의 add변수에  a,b값은 10, 20으로 각각 선언!
console.log(sum) --> 30 //sum값 나옴!
```
#### 2. 즉시 실행 함수
  * 함수를 정의함과 동시에 실행하는 함수 <br><br>
```javascript
사용법

1.
(function(매개변수) {
  ......
}(인수)); 
2. 
(function() {
  ......
})();
```
```javascript
사용예시

let result = (function(a, b) { //result변수에 익명함수를 할당함과 동시에 즉시실행함수 사용!
  return a + b; //함수 밖으로 result값을 표시하기위한 반환!
}(10, 20)); // a, b에 각각 10, 20할당!

console.log(result); --> 30
```
#### 3. 화살표 함수
  * 더 간단하게 함수작성을 할 수 있다! 익명함수에서만 사용이 가능함 <br><br>
```javascript
매개변수가 없을때

let hi = function() {
  return "Hello?";
}

줄여가는 과정
1.
let hi = () //function은 "="으로 생략하고 괄호안에 매개변수를 넣어준다!, 매개변수가 없으면 빈칸으로! => {return "Hello?"} 
// "=>"로 함수선언!
 
2. 
let hi = () => "Hello?"; //중괄호 안의 내용이 한줄뿐이라면 중괄호 생략가능!
```
```javascript
매개변수가 1개일때

let sum = function(a) {
  document.write("0에 " + a + "를 더한값은 " + a + "이다")
}
줄여가는 과정
1. 
let sum = (a) //function은 "="으로 생략하고 괄호안에 매개변수를 넣어준다! => {document.write("0에 " + a + "를 더한값은 " + a + "이다")}; 
// "=>"로 함수선언!

2. 
let sum = (a) => document.write("0에 " + a + "를 더한값은 " + a + "이다"); //중괄호 안의 내용이 한줄뿐이라면 중괄호 생략가능!
```
```javascript
매개변수가 2개일때

let add = function(a, b) {
  return a + b;
}

줄여가는 과정
1.
let add = (a,b) //function은 "="으로 생략하고 괄호안에 매개변수를 넣어준다! => {return a + b}; 
// "=>"로 함수선언!

2.
let add = (a,b) => return a + b; //중괄호 안의 내용이 한줄뿐이라면 중괄호 생략가능!
```
```javascript
중괄호 안의 식이 2개 이상일때

let add = function(a, b) {
  let sum = a + b;
  console.log(sum);
  return sum;
}

줄이는 법 
let add = (a,b) => {
  let sum = a + b;
  console.log(sum);
  return sum;
}
```
- - - -

## 2. Today I found out!!
모르는것은 ChatGpt에게 물어보니 잘 알려준다! 물론 초보자인 내가 오류를 발견할 만큼 오류가 잦긴하지만 지식에 관한것은 <Br>
대부분 정확한것같다! <br>
챗 지피티에게 대부분 물어봐서 정답을 얻었으니..!
- - - -

## 3. 오늘 읽은 자료 (혹은 참고할 링크, 생략해도 됨)
[블록스코프와 함수스코프 차이](https://mong-blog.tistory.com/entry/%EB%B8%94%EB%A1%9D-%EC%8A%A4%EC%BD%94%ED%94%84-%ED%95%A8%EC%88%98-%EC%8A%A4%EC%BD%94%ED%94%84%EC%9D%98-%EC%B0%A8%EC%9D%B4-javascript?category=967416) <br>
[return의 역할!](https://kyounghwan01.github.io/blog/JS/JSbasic/returnRoleFunction/)<br>
- - - -
 
## 4. 오늘의 프로젝트!
- - - -
## 5. 숙제!


