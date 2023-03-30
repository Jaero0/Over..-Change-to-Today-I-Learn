# 일일회고

## 목적
배우고 직접 적어보지 않으면 까먹는다   
그러므로 노트든 블로그든 어디든 배운 내용을 적어가며 암기한다   
그래서 난 깃허브 daily commit을 선택했다   
복습! 반복!

## 개인 회고 (20, 03, 2023)
집중력이 오늘은 딸린다.. 거의 3시간동안 4-1에서 4-4까지밖에.. 하지만 자랑스럽게도 마무리 했다! 그것으로 만족한다! 잘했다 나 자신! 기특하다!
- - - -
# 3/20(월)

## 1. Today I learned
### 1. JavaScript If, If~else 조건문
#### 1. 단순 조건에 맞는지만 확인하려면 if문을, 조건에 맞춰 참과 거짓을 구분해야하면 if~else문 사용
##### 1. if문 
  * if(조건){소스}, 소괄호안의 조건이 참이면 중괄호 안의 소스를 실행하고 거짓이면 무시함. <br><br>
##### 2. if~else문
  * if(조건){소스} else{소스}, 조건을 확인해 조건이 참일때와 거짓일때 실행할 명령어 따로! <br><br>
##### 3. if~else문 사용 주의사항!
  * 프로그램 실행속도의 차이를 위해! if~else문은 if에서 else로, if가 참이면 else를 무시한다는걸 이용하기! <br><br>
    * --> if(num == null){}else{} : 만약 입력을 취소할때는 1번의 실행이지만 입력을 실행하면 if문을 넘어 else까지 간다. <br>
    그렇게 되면 여러번의 입력을 실행했을때, 더 많은 횟수로 조건식을 읽어야하고 실행속도가 늦어지게 됨. <br><br>
    * --> if(num != null){}else{} : 만약 입력을 취소하면 1번의 실행으로 바로 else문으로 끝낼 수 있고, 입력을 실행한다 해도 <br>
    if문 안에서만 조건을 읽기때문에 더 빠른 실행속도로 else까지 갈 필요없이 실행할 수 있게됨! <br><br>
##### 4. JavaScript 조건연산자 (? : :(조건)?(true일때):(false일때))
  * 조건이 하나이고 실행할 명령도 하나일때 조건연산자 **? :** 를 사용하는게 간단.<br><br>

### 2. JavaScript Switch문
 * 조건이 3개 이상일때, if~else문으로 계속 쌓아가다보면 조건도 많아지고 오루가 생겼을때 찾기도 힘들어짐! 그럴땐 Switch문(door아님)으로!<br><br>
 * switch(변수) {case "1" : (---); break; case "99" : (---); break; default: \----;}<br><br>
 * [switch문 예제(지금은 몇월?)](https://github.com/Jaero0/DailyCommitBeginner_till_ExpertBackend/blob/main/Projects/switch-%EC%9B%94%20%EC%98%81%EC%96%B4%EB%A1%9C%3F.html)

 
### 3. JavaScript For반복문
 * 만약 1부터 100까지의 합을 구한다고 했을때, 연산자를 사용하려면 복잡하다! 그럴땐 for반복문!<br><br>
 * for(카운터변수; 조건식; 카운터변수조절){반복실행문} --> ex) for(var i = 1; i <101; i++ _**<-- 전위를 쓰면 식이 한번 읽히기 전에 i값이 올라감**_){기존변수 += i;}<br><br>
 * [for~of문](https://mi2mic.tistory.com/218) : for(var 변수 of 미리선언된 배열){document.write(변);} --> 값이 끝날때까지 미리선언된 배열을 반복함.
- - - -

## 2. Today I found out!!
for반복문 안의 for반복문은 굉장히 복잡하다! <br>
하지만!!! <br>
**바깥에 있는 for문이 한 번 실행될 때 마다
안에 있는 for문이 모든 반복을 마치는 동작을 하게 된다!!** <br>
을 기억하자 ㅇㅅㅇ
- - - -

## 3. 오늘 읽은 자료 (혹은 참고할 링크, 생략해도 됨)
[switch case문 예제](https://wikidocs.net/263) <br>
[for~of문](https://mi2mic.tistory.com/218) <br>
[for중첩 반복문](https://colossus-java-practice.tistory.com/40) 생각보다 복잡하니 자주 확인하자! <br>

- - - -
 
## 4. 오늘의 프로젝트!
[switch문 예제(지금은 몇월?)](https://github.com/Jaero0/DailyCommitBeginner_till_ExpertBackend/blob/main/Projects/switch-%EC%9B%94%20%EC%98%81%EC%96%B4%EB%A1%9C%3F.html) <br>
[피라미드 찍기!](https://github.com/Jaero0/DailyCommitBeginner_till_ExpertBackend/blob/main/Projects/%ED%94%BC%EB%9D%BC%EB%AF%B8%EB%93%9C%20%EC%B0%8D%EA%B8%B0.html) <br>

- - - -
## 5. 숙제!
 1. for 반복문으로 구구단 직접 만들어보기!
   * [이 자료 사용!](https://github.com/Jaero0/DailyCommitBeginner_till_ExpertBackend/blob/main/Projects/%EA%B5%AC%EA%B5%AC%EB%8B%A8%20%EC%88%99%EC%A0%9C!.html)
 2. 천천히 2스트라이크3볼 게임 만들어보기!
 3. \* 7개짜리 피라미드 7개, 직각삼각형, 정삼각형, 다이아몬드, 리본 등등 출력해보기!
   * [이 자료 사용!](https://github.com/Jaero0/DailyCommitBeginner_till_ExpertBackend/blob/main/Projects/%ED%94%BC%EB%9D%BC%EB%AF%B8%EB%93%9C%20%EC%88%99%EC%A0%9C!.html) 
