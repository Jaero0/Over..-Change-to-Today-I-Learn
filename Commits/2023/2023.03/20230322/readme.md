# 일일회고

## 목적
배우고 직접 적어보지 않으면 까먹는다   
그러므로 노트든 블로그든 어디든 배운 내용을 적어가며 암기한다   
그래서 난 깃허브 daily commit을 선택했다   
복습! 반복!

## 개인 회고 (22, 03, 2023)
캬.. 오늘 일하는데 겁나 짜증나는일이 많았다. 하지만 코딩공부를 하니 머리가 맑아짐! 아마 아무런 해답없이 몇개의 문제를 오로지 <br>
나의 힘으로만 풀어내었기 때문 아닐까? 정말 보람차다! <br>
그럼 이만 다시 스페인어 공부를하러...
- - - -
# 3/22(수)

## 1. Today I learned
### 1.  JavaScript do---while문<br><br>
 * while문 : while(조건식) {자바스크립트 소스 실행} <br><br>
 ex) while(i<5) {doc.writ("if true, keep repeat!"); i+=1;}
 조건식을 일차로 확인하고, 후에 소스를 실행.(소스를 실행할땐 꼭 변수의 반복횟수를 제어해줘야함!)<br><br>
 * for, while, do~while문의 차이!
  1. for반복문 : 초깃값이 있고, 일정한 간격으로 반복을 실행함!, 반복횟수가 정해져 있어서, 1부터 100까지의 합과같은 반복문 처리에 용이!, 반복횟수를 알고있을때!<br><br>
  2. while반복문 : 초깃값 없고, 일정한 간격으로 반복 하지 않아도됨!, 반복횟수가 가변적임! 1번일수도, 100번일수도, 1000...000번일수도!<br><br>
  그래서 **사용자의 입력같이 언제 발생할지 모르는 조건에 대해 반복해야할때!** 사용!<br><br>
  3. do~while반복문 : while반복문과 비슷하지만, while반복문은 문장의 실행부터 참-거짓을 따지는 반면, do while문은 무조건 첫 한번은 실행하고, 그다음부터 조건식을 따진다!<br><br>

### 2. JavaScript break문과 continue문<br><br>
  1. braek : 반복문 중간에 break문을 만나면 바로 밖으로 그 지점에서 빠져나온다! <br><br>
     * ex) for(var i = 1; i < 10, i++) { blablabalbal; break;} --> break에서 반복문 바로 종료!<br><br>
  2. continue : 반복문 중간에 continue문을 만나면 그 반복문장을 건너뛰고 반복문의 맨 앞으로 돌아간다!<br><br>
     * ex) for(var i = 1; i < 10, i++) { blablabla; continue; ~~ablablablablabal~~} --> 마지막 blabla가 continue때문에 계속 건너뛰어짐<br><br>
     * [짝수더하기](https://github.com/Jaero0/DailyCommitBeginner_till_ExpertBackend/blob/main/Projects/%EC%A7%9D%EC%88%98%EB%8D%94%ED%95%98%EA%B8%B0.html)<br><br>
 
### 3. 

## 2. Today I found out!!
  1. 팩토리얼은 머릿속으로 생각하기에 굉장히 간단하지만, 코드로 짜기에는 너무 어렵다! <br>
  2. 알고리즘 공부는 필수다! 복붙만 해서는 실력이 늘지않아! 알고리즘이 쓰러지지 않아!
- - - -

## 3. 오늘 읽은 자료 (혹은 참고할 링크, 생략해도 됨)
[vscode에서 nodejs열기!](https://kimvampa.tistory.com/101)
- - - -
 
## 4. 오늘의 프로젝트!
[프취달배 별찍기 10개 반쪽다이아몬드 2개 출력](https://github.com/Jaero0/DailyCommitBeginner_till_ExpertBackend/blob/main/Projects/%EB%B3%84%EC%B0%8D%EA%B8%B0/%ED%94%84%EC%B7%A8%EB%8B%AC%20%EB%B3%84%EC%B0%8D%EA%B8%B0%EB%AC%B8%EC%A0%9C.html)<br>
<br>
[짝수들의 합!](https://github.com/Jaero0/DailyCommitBeginner_till_ExpertBackend/blob/main/Projects/%EC%A7%9D%EB%8D%94/%EC%A7%9D%EC%88%98%EB%8D%94%ED%95%98%EA%B8%B0.html) <br><br>
[?의 배수구하기!](https://github.com/Jaero0/DailyCommitBeginner_till_ExpertBackend/blob/main/Projects/%3F%EC%9D%98%20%EB%B0%B0%EC%88%98%20%EA%B5%AC%ED%95%98%EA%B8%B0.html) <br><br>
[팩토리얼 구현!](https://github.com/Jaero0/DailyCommitBeginner_till_ExpertBackend/blob/main/Projects/factos!.html) <br><br>
[짝, 홀 구별!](https://github.com/Jaero0/DailyCommitBeginner_till_ExpertBackend/blob/main/Projects/%EC%A7%9D%2C%20%ED%99%80%20%ED%8C%90%EB%B3%84.html)
- - - -
## 5. 숙제!
1. 구구단과 팩토리얼의 논리구조는 나에게 너무나도 큰 벽이었다! 
   * [그래도 내일 다시 팩토리얼은 도전해보자!](https://github.com/Jaero0/DailyCommitBeginner_till_ExpertBackend/blob/main/Projects/factos!.html)<br><br>
2. 짝수들의 합, 홀수들의 합 구하기 프로그램!
   * [짝수더하기는 쉬운편!](https://github.com/Jaero0/DailyCommitBeginner_till_ExpertBackend/blob/main/Projects/%EC%A7%9D%EB%8D%94/%EC%A7%9D%EB%8D%94%EC%88%99%EC%A0%9C.html)<br><br>
3. [배수구하기 숙제](https://github.com/Jaero0/DailyCommitBeginner_till_ExpertBackend/blob/main/Projects/%EB%B0%B0%EC%88%98%EA%B5%AC%ED%95%98%EA%B8%B0/%EB%B0%B0%EC%88%98%EA%B5%AC%ED%95%98%EA%B8%B0%20%EC%88%99%EC%A0%9C.html)<br><br>
4. [홀짝판별숙제](https://github.com/Jaero0/DailyCommitBeginner_till_ExpertBackend/blob/main/Projects/%ED%99%80%EC%A7%9D/%ED%99%80%EC%A7%9D%ED%8C%90%EB%B3%84%EC%88%99%EC%A0%9C.html)
- - - -

