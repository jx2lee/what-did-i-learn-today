# What did I learn today 🩸

![](./img/logo.png)

- 그 날 이재준은 무엇을 배웠는가?
- 주말은 그렇다쳐도 주중에는 컴퓨터 끄기 전 꼭 commit 한다.
- 잔디밭을 채워보는게 목표이다.
- 하루 일과를 마치고 느낀점을 작성한다. 꼭 학습에 대한 회고가 아니어도 좋다.

# TOC

<details>
<summary> 2022.04 </summary>

- [2022.04.04](#20220404)
- [2022.04.05](#20220405)
- [2022.04.06](#20220406)
- [2022.04.07](#20220407)
- [2022.04.08](#20220408)
- [2022.04.10](#20220410)
- [2022.04.11](#20220411)
- [2022.04.12](#20220412)
- [2022.04.13](#20220413)
- [2022.04.15](#20220415)
- [2022.04.17](#20220417)
- [2022.04.22](#20220422)

</details>

# DAY

## 2022.04.04
- 클린 코더스 강의
  - [클린 코더스 강의 1.소개 및 OOP](https://www.youtube.com/watch?v=60lLSe1phks)
  - [클린 코더스 강의 2. OOP Part2](https://www.youtube.com/watch?v=D8_mbdoGPrg)
- [getting-started-with-mongodb](https://github.com/jx2lee/getting-started-with-mongodb)
  - capped collection 작성 완료
- interview scan: 속독 1회
- 운영에 사용되는 개발 test code 작성
  - service layer 의 테스트 코드 작성
  - 레퍼런스
    - [https://spring.io/guides/gs/testing-web](https://spring.io/guides/gs/testing-web)
    - [https://www.testwithspring.com/lesson/introduction-to-junit-4-test-classes](https://www.testwithspring.com/lesson/introduction-to-junit-4-test-classes/)
  - 뼈대 생성 완료, 내일은 count 진행
- groovy 에서 타 library import 하는 방법 search
  - 방법은 없어보임
  - 우선 test code 작성을 위해 레퍼런스 내용 참고하여 간단한 테스트 코드 구현 예정
  - 레퍼런스
    - [https://dev.to/kuperadrian/how-to-setup-a-unit-testable-jenkins-shared-pipeline-library-2e62](https://dev.to/kuperadrian/how-to-setup-a-unit-testable-jenkins-shared-pipeline-library-2e62)

### 회고
- 학습 스케줄링이 필요한 것 같다.
- 주기적인 학습
  - mongodb document 한긇화 작업 & 학습
  - 한가지 더 추가하면 좋을듯. hadoop?
- 그때그때 학습
  - 업무하면서 필요한 내용들을 정리
  - github 으로 관리하든, blog 로 작성하든 3일에 한 번 작성하면 좋을 듯
  - 아참, 도메인 구매해야지..

## 2022.04.05
- 클린 코더스 강의
  - [클린 코더스 강의 3. Function](https://www.youtube.com/watch?v=GYNT7O3rLhU)
    1. 원칙
    2. first rule of functions
       - 큰 함수를 보면 클래스로 추출할 생각을 해야함 (extract method object)
    3. example (fitness example)
       - [git](https://github.com/msbaek/fitness-example)
  - [클린 코더스 강의 4. Function Part2](https://www.youtube.com/watch?v=yd2xcVn_pAc)
    - `function should do one thing, do it well, do it only`
- [getting-started-with-mongodb](https://github.com/jx2lee/getting-started-with-mongodb)
  - Documents: field name 까지 완료
    - ., $ 표현이 들어간 field 네이밍은 권장하지 않음
- interview scan: 속독 2회
- QEMU guest agent
  - [https://docs.openshift.com/container-platform/4.7/virt/virtual_machines/virt-installing-qemu-guest-agent.html](https://docs.openshift.com/container-platform/4.7/virt/virtual_machines/virt-installing-qemu-guest-agent.html)
  - 운영 서비스 내 salt -> QEMU 로 전환하는 작업 확인, 위 기술 stack 살펴볼 필요 있음
  - 개인블로그에 짤막히 업로드 (예정)
- tclcs-metering-checker
  - CountMeteringReportServiceTest
  - 간단히 테스트를 완성했는데.. 테스트 코드를 이렇게 작성해도 되는지 개발팀 친한 전임님에게 시간되면 문의하기
  - 문의하고 SizeMeteringReportServiceTest 도 작성해보자

## 2022.04.06
- 클린 코더스 강의
  - [클린 코더스 강의 5. Function Structure](https://www.youtube.com/watch?v=JSV_YpTFhtw)
    - [자료](https://github.com/msbaek/clean-coders-2013/blob/master/3.Function%20Structure.png)
      - [x] 자로 따라하기: [https://github.com/jx2lee/videostore](https://github.com/jx2lee/videostore)
    - 객체지향(OO)의 가장 큰 장점은 **의존성 관리**
- [getting-started-with-mongodb](https://github.com/jx2lee/getting-started-with-mongodb)
  - Documents
- [java enum](https://docs.oracle.com/javase/tutorial/java/javaOO/enum.html)
  - 변수가 미리 정의된 상수 집합이 될 수 있도록 하는 특수한 데이터 유형
  - 변수는 변수에 대해 미리 정의된 값 중 하나여야 함
    - 일반적인 예로는 나침반 방향(NORTH, SOUTH, EAST 및 WEST 값)과 요일
  - 상수이기 때문에 필드 이름은 **대문자**
  - enum class 에 메서드 및 기타 필드를 포함할 수 있음
  - 컴파일러는 enum 을 만들 때 몇 가지 특수 메서드를 자동으로 추가
    - 예를 들어, 선언된 순서대로 enum 값을 포함하는 배열을 반환하는 정적 메서드 존재
    - for-each 구문과 조합하여 enum 값을 반복하는 데 사용
  - 링크에 나와있는 요일/행성 예제 따라해보는것도 좋을듯 함
    - [ ] [getting-started-with-java](https://github.com/jx2lee/getting-started-with-java)
- [mockito stubbing](https://javadoc.io/doc/org.mockito/mockito-core/latest/org/mockito/Mockito.html#2)

### 회고
- 역시 계획은 거창했지만 100프로 완료하지 못했다.
- 내일은 할 수 있는 만큼 계획을 잡아야겠다.

## 2022.04.07
- [ ] [클린 코더스 강의](https://www.youtube.com/playlist?list=PLeQ0NTYUDTmMM71Jn1scbEYdLFHz5ZqFA)
- [ ] [getting-started-with-mongodb](https://github.com/jx2lee/getting-started-with-mongodb)
- [ ] [java enum](https://docs.oracle.com/javase/tutorial/java/javaOO/enum.html)
  - [getting-started-with-java](https://github.com/jx2lee/getting-started-with-java)

### 회고
- 4월 7일은 제대로 공부하지 못했다. 업무도 많이 바빴고.. 컨디션이 좋지 못해 저녁에 푹 쉬었다.
- 8일부터는 빡공해야겠다.

## 2022.04.08
- [x] [클린 코더스 강의](https://www.youtube.com/playlist?list=PLeQ0NTYUDTmMM71Jn1scbEYdLFHz5ZqFA)
  - [클린 코더스 강의 5. Function Structure Part2](https://www.youtube.com/watch?v=cgiDv1XFWsk)
    - [checked vs unchecked exception](https://madplay.github.io/post/java-checked-unchecked-exceptions)
      - `RuntimeException` 을 상속한 클래스를 Unchecked Exception, 상속하지 않은 클래스를 Checked Exception
      - Unchecked Exception 은 명시적으로 예외 처리를 하지 않아도 됨
      ![Java Exception 구분](https://madplay.github.io/img/post/2019-03-02-java-checked-unchecked-exceptions-1.png)
    - [ ] [실습](https://github.com/jx2lee/stack-example)
- [x] [java enum](https://docs.oracle.com/javase/tutorial/java/javaOO/enum.html)
  - [getting-started-with-java](https://github.com/jx2lee/getting-started-with-java/commit/5a37d124e398ceb1cbb7895ede8e5aa8d34fcd0c)
- [x] 개인 블로그 댓글 utterances 작업
- [ ] [getting-started-with-mongodb](https://github.com/jx2lee/getting-started-with-mongodb)

### 회고
- 목표를 모두 완료하지 못했다.
- 못한 부분은 다음날 꼭 마무리할 수 있도록 진행해야겠다.

## 2022.04.10
- [x] jenkins shared library 개발 환경 구성
- [x] [실습](https://github.com/jx2lee/stack-example)
  - [github commit](https://github.com/jx2lee/stack-example/commits/practice/jx2lee)

### 회고
- 일요일이라 살짝 공부했다.
- 사실 stack-example 은 월요일날 마무리를 했다.. 월요일은 항상 바쁜 것 같다.

## 2022.04.11
### 회고
- 저녁먹고 클린 코더스 강의를 듣다 너무 졸려 30분 잠을 청했는데.. 눈떠보니 새벽이었다.
- 할 수 있는 범위만큼 선정하는게 중요한 것 같다.

## 2022.04.12
### 회고
- 오랜만에 출근해서 바쁘게 보냈다. 새벽운동을 하지 못해서 저녁에 운동을 하니.. 공부할 여력이 없었다.
- smtp 서버를 local 로 띄우는 방법(with postfix) 을 조금 살펴보고 취침할 예정이다.
- 1년간 비대면으로 협업하던 개발팀분을 처음으로 만났다. 끊임없는 개선 의지를 보고 배울점이 많다고 느낀 하루였다.

## 2022.04.13
- [x] [클린 코더스 강의](https://www.youtube.com/playlist?list=PLeQ0NTYUDTmMM71Jn1scbEYdLFHz5ZqFA)
  - [클린 코더스 강의 6. Form](https://www.youtube.com/watch?v=cgiDv1XFWsk)
  - [ ] markdown 정리: [commit link](https://github.com/jx2lee/clean-coders-2013/commit/92e126510cc1b1526a8ad343ad2b07c119d449f4)
    - 남은 부분 내일 정리
- [x] [getting-started-with-mongodb](https://github.com/jx2lee/getting-started-with-mongodb)

### 회고
- 마크다운으로 정리하는 시간이 오래걸렸다. 업무 시간 내 여유로우면 작업을 진행해야겠다.
- 로컬 smtp 서버를 구축하고 테스트가 필요할 것 같다. 메일이 정상발송 되면 PR 올려도 좋을 듯 싶다.

## 2022.04.14
### 회고

## 2022.04.15
- [x] 클린 코더스 강의 Forms 마크다운 정리
  - 완료
  - [링크](https://github.com/jx2lee/clean-coders-2013/commit/8eb2f07a9b603475b4cbac818c26833c05b051e9)
- [x] local smtp 세팅 with Dooray
  - 받는 메일을 gmail 로 할 때는 가능
  - 사내 메일로 하면 실패인데.. 이 부분 확인 필요
  - 우선 hotfix 내용은 정상적으로 반영됨
- [] [getting-started-with-mongodb](https://github.com/jx2lee/getting-started-with-mongodb)

### 회고
- 드디어 로컬 smtp 서버 구성을 완료했다.
- 회사 도메인으로 메일이 발송되는 것도 확인하였다. 내일은 postfix 로 로컬 smtp 설정하는 글을 작성할 계획이다.

## 2022.04.16
- [x] 야나두: 9강까지 완료
  - `from here on out`: 이제부터는
  - `by the way`: 그나저나/근데 말이지/근데 있잖아
    - 앞 뒤 모두 사용 가능
  - `(Oh,) I'm very sorry`: 유감이에요
    - 대답: `Thank you` 
  - `There, there`: 그래 그래, 옳지 옳지
    - 위로, 사운드로 생각
    - `There you go`: 잘했어
  - `I think i just peed a little`: 정말 끝내준다 (소변 흘릴 만큼..?)
- [x] blog post 작성: postfix
  - [https://jx2lee.github.io/etc-postfix-with-mac](https://jx2lee.github.io/etc-postfix-with-mac)
- [x] tclcs-metering-checker
  - countMeteringReportService.makeReportAndNotify 시 enum 을 파라미터로 받고 있음
  - mock 으로 대체하려고 했지만 버전 문제로 enum mock 이 불가
    - [참고](https://stackoverflow.com/questions/14292863/how-to-mock-a-final-class-with-mockito)
    - mockito-inline 의존성을 추가하면 되지만.. 혹시 모를 문제를 대비하고자 다른 방법이 있는지 확인 예정
    - 완료되면 SizeMeteringReportServiceTest 도 작성완료할 예정
- [x] vue
  - [코딩애플](https://www.youtube.com/playlist?list=PLfLgtT94nNq3Br68sEe26jkOqCPK_8UQ-)
    - [https://www.youtube.com/watch?v=-tVaahsXpwk&list=PLfLgtT94nNq3Br68sEe26jkOqCPK_8UQ-&index=2](https://www.youtube.com/watch?v=-tVaahsXpwk&list=PLfLgtT94nNq3Br68sEe26jkOqCPK_8UQ-&index=2)
    - [https://www.youtube.com/watch?v=NONWar0jGLM&list=PLfLgtT94nNq3Br68sEe26jkOqCPK_8UQ-&index=2](https://www.youtube.com/watch?v=NONWar0jGLM&list=PLfLgtT94nNq3Br68sEe26jkOqCPK_8UQ-&index=2)
    - 개발환경 세팅 완료, 우선은 간단한 예제를 통해 vue 맛보고 inflearn 강의 듣기!

### 회고
- 운영업무 개발에 대한 학습을 진행했다. postfix 가 정상적으로 동작하여 메일을 드디어 받아보았다.
- 사내에서 사용중인 vue 를 한번쯤 살펴보면 좋을 것 같아 코딩애플 유튜브를 시청했다. 빠르게 살펴보고 inflearn 에서 깊이있게 학습할 예정이다.
- spring mvc & jpa 복습을 진행해야겠다. (벌써 AOP 도 까먹은 듯 하다. 반복이 중요한 듯)

## 2022.04.17
- [x] 야나두
  - `I just was like` (행동/소리): 내가 막 이랬어
  - `on the side`: 따로 주세요
  - `I just got ~`: 이제 막(just) ~를 알겠어
  - `as good as ~`: ~만큼 좋다
    - `This is as good as That`: 저것보다 좋다
- [x] vue: [코딩애플](https://www.youtube.com/playlist?list=PLfLgtT94nNq3Br68sEe26jkOqCPK_8UQ-)
  - [Vue 3강: v-for 반복문 보니까 HTML도 프로그래밍 언어네](https://www.youtube.com/watch?v=T4N9wjx7_E4)
  - [Vue 4강: 이벤트 핸들러로 허위매물 신고버튼 만들기](https://www.youtube.com/watch?v=Agm-F366ZwY)
- [x] [고승범 kafka 강의: virtual meetup 3rd 2021](https://www.youtube.com/watch?v=1NgWYemxCo8)

### 회고
- vue 학습을 진행했다. 사내 프론트가 vue 로 되어 있는데 프론트쪽도 학습하면 분명 도움이 될 것 같다.
- 영어공부는 깜빡하지 말고 매일 해보기!

## 2022.04.22
- [x] jenkins shared library 개발
  - 다중 dooray notify 개발
  - 테스트코드 작성 필요
- [x] [getting-started-with-mongodb](https://github.com/jx2lee/getting-started-with-mongodb)
  - documents 페이지 업로드
  - [commit](https://github.com/jx2lee/getting-started-with-mongodb/commit/b505318dae88e403bf273792f6d3c3943b71f6ea)
- [x] (복습) 스프링 웹 MVC-1
  - html response 테스트코드 작성
    - PrintWriter 테스트 코드 example 확인 및 적용
      - [링크](https://github.com/cschneider/osgi-testing-example/blob/master/src/test/java/net/lr/example/testing/PrimeCalculatorServletTest.java)
- [] 야나두

### 회고
- 오랜만에 데일리로그를 작성했다.
- 주말에도 공부했지만.. 적지 못했다. 새로운 것을 배워가며 복습도 놓치지 않고 진행해야겠다.
