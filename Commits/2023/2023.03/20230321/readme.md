# 일일회고

## 목적
배우고 직접 적어보지 않으면 까먹는다   
그러므로 노트든 블로그든 어디든 배운 내용을 적어가며 암기한다   
그래서 난 깃허브 daily commit을 선택했다   
복습! 반복!

## 개인 회고 (21, 03, 2023)

- - - -
# 3/21(화)
**오늘은 별찍기 문제만 푸는데 거의 2시간, 그리고 메타인지를 통한 무엇이 부족한지를 알아냈다!** <br>
**후에 자료구조와 알고리즘을 공부하자! 그리고 내일은 구구단 숙제 및 4-5~4문제까지 완료하기!**
## 1. Today I learned
### 1. 복습! 복습만 하는데 굉장한 시간이 걸렸다!

### 2. JavaScript do---while문
 * while문 : while(조건식) {자바스크립트 소스 실행} <br>
 ex) while(i<5) {doc.writ("if ture, keep 
 
### 3. 

## 2. Today I found out!!
  1. switch case 문을 사용할때는 변수로 호출하기! + 변수가 문자열이면 case에도 문자열로 입력해주기!
  2. [for문 별찍기 프로젝트 확인!](https://github.com/Jaero0/DailyCommitBeginner_till_ExpertBackend/tree/main/Projects/%EB%B3%84%EC%B0%8D%EA%B8%B0) <br>
     * 별찍기는 쥰...내게 어렵다! 언젠간 괜찮아 지겠지? 프로그래밍 논리여 길러져라!!
     * 정삼각형 별찍기는 아직 나에게 무리.. 이걸 완료하면 알고리즘에 대해 파악이 가능해진다하니.. 천천히 도전해보자!
     * 일단 Js, Jquery 공부를 끝낸 후 알고리즘 공부 드가자! 기초 문법만 탄탄하게 쌓아놓고 백준 알고리즘문제, 파이썬 자료구조&알고리즘 책 사서 공부!
- - - -

## 3. 오늘 읽은 자료 (혹은 참고할 링크, 생략해도 됨)
[협업을 위한 vscode 설정!](https://overcome-the-limits.tistory.com/entry/%ED%98%91%EC%97%85-%ED%98%91%EC%97%85%EC%9D%84-%EC%9C%84%ED%95%9C-VScode-%EC%84%A4%EC%A0%95) <br>

- - - -
 
## 4. 오늘의 프로젝트!
[for반복문으로 다이아몬드찍기 with CSS!](https://github.com/Jaero0/DailyCommitBeginner_till_ExpertBackend/blob/main/Projects/%EB%B3%84%EC%B0%8D%EA%B8%B0/%EB%8B%A4%EC%9D%B4%EC%95%84%EB%AA%AC%EB%93%9C%20with%20css.html) <br>
[for반복문으로 피라미드 7개 출력 with CSS!](https://github.com/Jaero0/DailyCommitBeginner_till_ExpertBackend/blob/main/Projects/%EB%B3%84%EC%B0%8D%EA%B8%B0/%ED%94%BC%EB%9D%BC%EB%AF%B8%EB%93%9C%207%EC%A4%84%20%20with%20css.html) <br>
[switch case문으로 ~월 영어로 출력!](https://github.com/Jaero0/DailyCommitBeginner_till_ExpertBackend/blob/main/Projects/Switch/switch%20Review.html)
- - - -
## 5. 숙제!
 1. 4-5 ~ 4문제까지 공부하고 커밋작성!
 2. 구구단 숙제하기! 이해 안되면 한번보고 완벽히 이해한 후 그 다음날 숙제로 한번더 해보기! 
- - - -
1. 편붕짱의 완벽한 다이아몬드 별찍기! 일단 체득 후 알고리즘 공부 후 다시 이해해보기!
```
public class Test {
    public static void main(String[] args) { 
        int star = 15; // 다이아몬드 가로세로 길이
        for(int i = 0; i < star; i++) {
            for(int j = 0; j < star; j++) {
                int half = star / 2;
                if(half-Math.abs(half-i) >= Math.abs(half-j)) System.out.print("*"); // 줄 바꿈 없이 별 출력, math.abs는 절댓값임!
                else System.out.print(" "); // 줄 바꿈 없이 빈칸 출력
            }
            System.out.println(); // 줄 바꿈
        }
        
    }
}
```
