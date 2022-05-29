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
- [2022.04.23](#20220423)
- [2022.04.24](#20220424)
- [2022.04.25](#20220425)
- [2022.04.28](#20220428)
- [2022.04.29](#20220429)
- [2022.04.30](#20220430)

</details>

<details>
<summary> 2022.05 </summary>

- [2022.05.03](#20220503)
- [2022.05.04](#20220504)
- [2022.05.05](#20220505)
- [2022.05.06](#20220506)
- [2022.05.09](#20220509)
- [2022.05.15](#20220515)
- [2022.05.16](#20220516)
- [2022.05.19](#20220519)
- [2022.05.20](#20220520)
- [2022.05.23](#20220523)
- [2022.05.26](#20220526)
- [2022.05.29](#20220529)

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

## 2022.04.23
- [x] 야나두
  - `get along`: ~와 어울리다, 사이좋게 지내다.
    - `get along with`: ~와 사이좋게 지내다.
    - e.g
      - we get along: 우린 사이가 좋아요.
      - they don't get along
  - `Bummer`: 아이고 저런
    - what a bummer: (강조해서) 아이고
    - I'm sorry: 조금 더 정중하고 예의를 갖출 때 사용하는 표현
  - `What's it say?`: 뭐라고 써져 있어?
    - say 를 적혀있다고 표현
    - e.g
      - what does he say?: 그 남자가 뭐라고 하는데?
      - what does the note say?: 노트에 뭐라고 적혀있는데? 
- spring 복습
  - [x] spring web mvc
    - servlet 테스트 코드 작성
    - 한 개 테스트 코드 작성 후 본 진도 나갈 수 있을 것으로 예상
  - [x] spring jpa
    - h2 를 docker 로 설치하려다 시간만 버렸다.
    - multipass 로 ubuntu vm 을 생성하였고 여기서 Container 를 관리해봐야겠다.
  - [] spring batch

### 회고
- spring batch 를 공부하지 못했다. mvc2 편도 언능 복습해야하는데.. 시간을 짧게 나눠 (최대 30분?) 여러 기술들을 복습해야겠다.
  - batch with jenkins 로 배치 스케쥴링 토이 프로젝트를 진행하면 좋을 것 같다.
  - 뭐가 있지..
- 데이터 엔지니어 역량 강화를 위해 필요한 것들을 리스트화 해야겠다.

## 2022.04.24
- [x] 야나두
  - `deal with`: ~을 처리하다.
    - e.g
      - I've got to deal with it: 내가 처리할 예정이야
  - `kill for`: 너무 ~ 하고싶다.
    - I would(`==I'd`) kill for a coffee break: 나 지금 너무 커피마시고 싶어
  - `Get yourself something`: (너 자신을 위해) ~라도 해 (something)
  - `Sorry, you were saying..`: 그래서 하던 말이 (뭐야)?
    - what were you saying?: 뭐라 그랬지? 위 문장을 의문문으로 응용
- spring 복습
  - [x] spring batch
    - PDF p.19
  - [x] spring mvc 1
    - 지금까지 공부해왔던 코드들에 대한 테스트 코드 작성 완료 (~108)
    - 내일부터는 진도 가능
  - [x] spring jpa
    - 이전에 올려놨던 코드들은 마지막 강의를 기준으로 최신화되어있음
    - 네이밍으로 main 분리 & 테스트코드 작성 필요
    - 우선 h2 docker 에 삽입되는 거 확인

### 회고
- spring 복습을 모두 완료했다. 내일부터는 복습이 가능한 환경을 구성했다.
- log 관리를 위한 서치가 필요하다. 기존에 눈여겨왔던 두 기술을 살펴볼 예정이다.
- 매일같이 스터디할 주제는 다음과 같이 정리했다.
  - mongodb
  - 클린 코더스 강의
  - 그동안 학습한 spring 복습 (mvc, jpa, batch: **얘는 강의보다는 강의자료로 진행 예정**)
  - 야.나.두

## 2022.04.25
- [] 야나두
- [x] [getting-started-with-mongodb](https://github.com/jx2lee/getting-started-with-mongodb)
  - MongoDB CRUD Operations 정리 중
  - Update 까지 작성 완료
- spring in action
  - [x] spring mvc-1
  - [] spring jpa
  - [] spring batch

### 회고
- 오늘도 고정 스터디를 마무리 못했다.
- 스케쥴 봐가면서 진행해야겠다..

## 2022.04.28
- [x] [클린 코더스 강의](https://www.youtube.com/playlist?list=PLeQ0NTYUDTmMM71Jn1scbEYdLFHz5ZqFA)
  - [5.TDD-Practice](https://www.youtube.com/watch?v=wmHV6L0e1sU&list=PLeQ0NTYUDTmMM71Jn1scbEYdLFHz5ZqFA)
  - 13:06
- [x] elasticsearch rolling restart
  - [https://jx2lee.github.io/es-shard-allocation](https://jx2lee.github.io/es-shard-allocation/)
  - 가이드로 등록하기 위한 서치
- [] 야나두
- [] [getting-started-with-mongodb](https://github.com/jx2lee/getting-started-with-mongodb)
- spring in action
  - [] spring mvc-1
  - [] spring jpa
  - [] spring batch

### 회고
- 갑자기 개인 블로그가 장애가 났다. node 버전이 바뀌어서 그런 것 같은데.. 우선 정상화 되었다.
  - 설정값들은 천천히 바꿔야지

## 2022.04.29
- [x] [getting-started-with-mongodb](https://github.com/jx2lee/getting-started-with-mongodb)
  - mongodb-crud-operations 작성 완료 및 commit
  - insert-documents 작성 중
- [x] [클린 코더스 강의](https://www.youtube.com/playlist?list=PLeQ0NTYUDTmMM71Jn1scbEYdLFHz5ZqFA)
  - [5.TDD-Practice](https://www.youtube.com/watch?v=wmHV6L0e1sU&list=PLeQ0NTYUDTmMM71Jn1scbEYdLFHz5ZqFA)
  - **TDD 절차** chapter 까지 완료
- [x] 야나두
  - `humiliating`: 창피하다
    - 발음은 휴밀리에이링
  - `I guess`: ~인 것 같아
    - 이후 새로운 문장이 나오는 케이스가 많음
  - `I'm in!`: 나 낄래!
    - `I'm out`: 나 빠질래..
- [x] es coordinate node 장애 분석
  - es cluster 장애가 난 것으로 분석
  - 태스크 작성 중
- spring in action
  - [x] spring mvc-1
    - dispatcher 테스트 코드 작성하는 example 을 찾아봐야함
  - [] spring jpa
  - [] spring batch

### 회고
- es cluster 장애가 발생하여 해당 장애를 분석하는 과정에 시간을 소요했다.
  - 원인을 파악하기 위해 모니터링 지표 & 로그를 확인하고 있다.
  - 블로그 포스팅 할 예정
- 고정 스터디를 계속해서 완료하고 있지 못했다. 다음주 일정이 몇 있어 더 못할 수 있으니 조금씩이라도 챙기자

## 2022.04.30
- [x] [leetcode](https://leetcode.com/problemset/algorithms)
  - [https://leetcode.com/problems/evaluate-division](https://leetcode.com/problems/evaluate-division/)
- [x] [getting-started-with-mongodb](https://github.com/jx2lee/getting-started-with-mongodb)
  - multipass 로 테스트 환경 구축 (ubuntu & docker)
  - markdown 작성 중
- [x] 블로그 복구
- [x] [클린 코더스 강의](https://www.youtube.com/playlist?list=PLeQ0NTYUDTmMM71Jn1scbEYdLFHz5ZqFA)
  - [5.TDD-Practice](https://www.youtube.com/watch?v=wmHV6L0e1sU&list=PLeQ0NTYUDTmMM71Jn1scbEYdLFHz5ZqFA)
  - 22:41, [github link](https://github.com/msbaek/tdd-practice)
- [] 야나두
- spring in action
  - [] spring mvc-1
  - [] spring jpa
  - [x] spring batch
    - p.19

### 회고
- 4월이 끝났다. 그동안 했던 내용들을 살펴보는데 조금 더 세심하게 챙겨야겠다.

## 2022.05.03
- [x] [leetcode](https://leetcode.com/problemset/algorithms)
  - [shortest-unsorted-continuous-subarray](https://leetcode.com/problems/shortest-unsorted-continuous-subarray/)
- [x] [SQL 쿡북](http://www.kyobobook.co.kr/product/detailViewKor.laf?ejkGb=KOR&mallGb=KOR&barcode=9791162245125&orderClick=&Kc=)
  - page 50까지 완료, 51부터 시작 예정
  - 틈날때마다 읽자
- [x] [getting-started-with-mongodb](https://github.com/jx2lee/getting-started-with-mongodb)
  - [insert-document 작성 완료](https://github.com/jx2lee/getting-started-with-mongodb/blob/main/mongodb-crud-operations/insert-documents.md)
  - 순서대로 하는 것보다.. 원리 기반 document 를 작성해보는 건 어떨까..? 라는 생각이 듬
- [x] [클린 코더스 강의](https://www.youtube.com/playlist?list=PLeQ0NTYUDTmMM71Jn1scbEYdLFHz5ZqFA)
  - [5.TDD-Practice](https://www.youtube.com/watch?v=wmHV6L0e1sU&list=PLeQ0NTYUDTmMM71Jn1scbEYdLFHz5ZqFA)
  - 27:40, [github link](https://github.com/msbaek/tdd-practice)
 
### 회고
- 각 스터디 마다 시간을 조금 줄여 우선은 완료하였다.
- ES circuit breaking exception 블로그 포스트 예정

## 2022.05.04
- [x] 야나두
  - `wash out`: (얼룩이나 자국을) 씻겨내다
    - 사람에게 쓸 때는 **기운이 없는, 지친**
  - `as A as B`: B 만큼 A 해
  - `Not a word`: 아무 말 하지마
  - `Should I know you?`: 제가 아는 분인가요?
    - 친근한 표현은 should -> do
- [x] [leetcode](https://leetcode.com/problemset/algorithms)
  - [max-number-of-k-sum-pairs](https://leetcode.com/problems/max-number-of-k-sum-pairs)
- [x] elasticsearch circuit breaking exception
  - 블로그 포스트 예정
  - 개요 작성
- [] [SQL 쿡북](http://www.kyobobook.co.kr/product/detailViewKor.laf?ejkGb=KOR&mallGb=KOR&barcode=9791162245125&orderClick=&Kc=)
  - page 50까지 완료, 51부터 시작 예정
  - 틈날때마다 읽자
- [] [getting-started-with-mongodb](https://github.com/jx2lee/getting-started-with-mongodb)
- [] [클린 코더스 강의](https://www.youtube.com/playlist?list=PLeQ0NTYUDTmMM71Jn1scbEYdLFHz5ZqFA)
  - [5.TDD-Practice](https://www.youtube.com/watch?v=wmHV6L0e1sU&list=PLeQ0NTYUDTmMM71Jn1scbEYdLFHz5ZqFA)
  - 27:40, [github link](https://github.com/msbaek/tdd-practice)

### 회고
- 역시 계획은 방대했다. 할 수 있는 만큼만 계획하자.
  - 단, 계획한 만큼은 모두 끝낼 것!

## 2022.05.05
- [x] [getting-started-with-mongodb](https://github.com/jx2lee/getting-started-with-mongodb)
  - replica set 작성중
- [] [클린 코더스 강의](https://www.youtube.com/playlist?list=PLeQ0NTYUDTmMM71Jn1scbEYdLFHz5ZqFA)
  - [5.TDD-Practice](https://www.youtube.com/watch?v=wmHV6L0e1sU&list=PLeQ0NTYUDTmMM71Jn1scbEYdLFHz5ZqFA)
  - 27:40, [github link](https://github.com/msbaek/tdd-practice)
- [x] 야나두
  - `selfie`: 우리가 흔히 알고있는 셀카
    - Can i take a selfie with you?: 같이 셀카 찍어도 될까요?
    - take a picture -> take a selfie
  - `window shopping`: 우리가 흔히 알고있는 아이쇼핑
    - Do you like to go window shopping?: 아이쇼핑 하는 거 좋아하니?

### 회고
- 오늘도 계획한 것들을 끝내지 못했다.
- **할 수 있는 만큼만 작성하자**

## 2022.05.06
- [x] 야나두
  - `single`: 흔히 알고있는 솔로
    - Are you single?: 너는 솔로니?
    - She is single, too: 그도 솔로야
    - He's been single for a while: 그는 솔로로 지낸지 좀 됐어
  - `combo || meal`: 흔히 알고있는 세트메뉴
    - I'd like to order a combo: 세트 하나 주문할게요
    - Can I get a combo?: 세트 하나 주시겠어요?
    - Can I have a chicken burger meal?: 치킨버거 세트 하나 주시겠어요?
      - Can I have == Can I get
- [x] [leetcode](https://leetcode.com/problemset/algorithms)
  - [string-to-integer-atoi](https://leetcode.com/problems/string-to-integer-atoi)
- [x] [SQL 쿡북](http://www.kyobobook.co.kr/product/detailViewKor.laf?ejkGb=KOR&mallGb=KOR&barcode=9791162245125&orderClick=&Kc=)
  - 아이디 변경으로 16일부터 대출 가능
- [x] elasticsearch circuit breaking exception
  - 블로그 포스트 업로드: [url](https://jx2lee.github.io/elasticsearch-circuit-breaking-exception)
- [x] [getting-started-with-mongodb](https://github.com/jx2lee/getting-started-with-mongodb)
  - replication 작성 중
  - 작성하다보니 어려운 부분이 많다.. 시간이 좀 걸릴 거 같다.
- [] [클린 코더스 강의](https://www.youtube.com/playlist?list=PLeQ0NTYUDTmMM71Jn1scbEYdLFHz5ZqFA)
  - [5.TDD-Practice](https://www.youtube.com/watch?v=wmHV6L0e1sU&list=PLeQ0NTYUDTmMM71Jn1scbEYdLFHz5ZqFA)
  - 27:40, [github link](https://github.com/msbaek/tdd-practice)

### 회고
- 금일은 계획한 일들을 대부분 마무리하였다. 각 항목 당 분배시간을 줄이니 완료할 수 있었다.

## 2022.05.09
- [x] 야나두
  - `Air conditioner`: 에어컨
    - Turn on the air conditioner, please: 에어컨좀 켜주세요
    - The air conditioner is not working well: 에어컨이 작동하지 않아요
  - `Remote control`: 리모컨
    - Give me the remote control: 리모컨 내놔
    - I can't find the remote control: 리코너이 안보이네
  - `Bottoms up`: 원샷
    - Everybody, bottoms up!
    - == Down it == Chug it
- [x] [leetcode](https://leetcode.com/problemset/algorithms)
  - [letter-combinations-of-a-phone-number](https://leetcode.com/problems/letter-combinations-of-a-phone-number)
- [] [getting-started-with-mongodb](https://github.com/jx2lee/getting-started-with-mongodb)
- spring in action
  - [X] spring mvc-1
    - jsp 테스트 코드 search
      - [stackoverflow](https://stackoverflow.com/questions/3031353/how-can-i-unit-test-a-jsp) 에 따르면.. jsp 소스를 테스트하려면 Selenium 또는 HttpUnit과 같은 클라이언트 측 테스트 프레임워크를 사용해야 한다고 한다.
      - jsp 로 짜여진 코드에 대한 테스트는 스킵하고 어떤 원리로 동작되는지는 내일부터 확인해보면서 학습할 예정이다.
  - [x] spring jpa
    - HelloJpaMain 테스트 코드 작성중
    - entitymanager 테스트 코드 search
  - [] spring batch
    - ~ p.19
- [] [클린 코더스 강의](https://www.youtube.com/playlist?list=PLeQ0NTYUDTmMM71Jn1scbEYdLFHz5ZqFA)
  - [5.TDD-Practice](https://www.youtube.com/watch?v=wmHV6L0e1sU&list=PLeQ0NTYUDTmMM71Jn1scbEYdLFHz5ZqFA)
  - 27:40, [github link](https://github.com/msbaek/tdd-practice)

### 회고
- 요새 정신이 없는 것 같다. 놓치지 않고 꾸준히 진행해야겠다.

## 2022.05.15
- [x] 야나두
  - `Go Dutch`: 더치페이
    - Shall we go Dutch on this?
    - Let's go Dutch == We should split the bill
    - I will treat you == I got you == It's on me: 내가 살게
  - `Convertible`: 오픈카
    - Did you see the newest convertible?: 새로운 오픈카 봤어?
    - The man is driving a convertible. 남자가 오픈카를 운전하고 있어.
  - `Hoodie`: 후드티
    - Hoodies look good on you: 후드티가 잘 어울려
    - I have a lot of hoodies: 난 후드티가 많아
- [x] [leetcode](https://leetcode.com/problemset/algorithms)
  - [populating-next-right-pointers-in-each-node-ii](https://leetcode.com/problems/populating-next-right-pointers-in-each-node-ii)
- [x] [SQL 쿡북](http://www.kyobobook.co.kr/product/detailViewKor.laf?ejkGb=KOR&mallGb=KOR&barcode=9791162245125&orderClick=&Kc=)
  - 내부 오류로 인해 학습이 불가능.. 내일 담당자에게 문의 예정
- [x] [클린 코더스 강의](https://www.youtube.com/playlist?list=PLeQ0NTYUDTmMM71Jn1scbEYdLFHz5ZqFA)
  - [5.TDD-Practice](https://www.youtube.com/watch?v=wmHV6L0e1sU&list=PLeQ0NTYUDTmMM71Jn1scbEYdLFHz5ZqFA)
  - 완료
    - repo 는 생성했지만 push 는 하지 않음
    - 추가작업이 있을 것 같아 Movie example 만 진행 완료
    - 이후 강의에서 진행하고 완료되면 push 예정
- spring in action
  - [x] spring mvc-1
    - p.131
    - front controller 테스트 코드 작성 중
  - [x] spring batch
    - p.49
    - 인프런 강의 실습에서 직접 진행할 것 (다음부터,,?)
  - [] spring jpa

### 회고
- 주말 이용해 jpa 제외하고 모두 완료했다.
- 월요일도 화이팅!

## 2022.05.16
- [x] 야나두
  - `wake-up call`: 모닝콜
    - Can I ask for a wake-up call?: 모닝콜 부탁할 수 있을까요?
    - I did not get my wake-up call today: 오늘 모닝콜을 받지 못했어요!
  - `Matching outfit`: 커플룩
    - How about matching outfit?: 커플룩 하는거 어때?
    - We wore matching outfit: 우리 커플룩 입었어
  - `actor(actress)/celebrity/star`: 탤런트
    - You look like an actor: 너 그 배우 닮았다.
    - I want to become an actor: 난 배우가 될거야
- [x] [leetcode](https://leetcode.com/problemset/algorithms)
  - [shortest-path-in-binary-matrix](https://leetcode.com/problems/shortest-path-in-binary-matrix)
  - 내일 로직 다시 검토 예정
- [x] [클린 코더스 강의](https://www.youtube.com/playlist?list=PLeQ0NTYUDTmMM71Jn1scbEYdLFHz5ZqFA)
  - [7.TDD-2](https://www.youtube.com/watch?v=c-Pv2ia05Ek&list=PLeQ0NTYUDTmMM71Jn1scbEYdLFHz5ZqFA&index=9&t=5s)
  - 19:24 // TyrantTest 코드 작성 중
    - assertThat 부분에서 기대한 결과값이 다르다고 오류 발생
    - 원인 파악중
- spring in action
  - [] spring jpa
  - [] spring mvc-1
    - p.131
    - front controller 테스트 코드 작성 중
  - [] spring batch
    - p.49

### 회고
- spring in action 부분은 내일 진행해야할 듯 싶다. 클린 코더스 강의 코드 중 테스트에 자꾸 실패하는 부분이 발생되어서... 요 부분 확인하는데 시간이 많이 소요되었다.
- elasticsearch 패캠 강의를 신청했다. mongodb 와 같이 병행하면 서비스 이해에 도움이 될 듯 하다. 
  - 정리가 필요한 부분은 블로그로 작성해놓을 예정

## 2022.05.19
- [x] 야나두
  - `COMMERCIAL`: CF
    - Have you seen the commercial?: 광고 봤어?
    - What is the commercial about?: 무슨 광고인데?
    - I love this commercial: 난 그 광고 좋아
  - `that hits the spot`: 그게 딱이었어 (해장할 때 뼈해장국 먹으면서 할 수 있음)
  - `I crave A`: A 가 땡긴다. crave 라는 단어
- [x] [leetcode](https://leetcode.com/problemset/algorithms)
  - [shortest-path-in-binary-matrix](https://leetcode.com/problems/shortest-path-in-binary-matrix)
  - 로직 확인
- [x] [클린 코더스 강의](https://www.youtube.com/playlist?list=PLeQ0NTYUDTmMM71Jn1scbEYdLFHz5ZqFA)
  - [7.TDD-2](https://www.youtube.com/watch?v=c-Pv2ia05Ek&list=PLeQ0NTYUDTmMM71Jn1scbEYdLFHz5ZqFA&index=9&t=5s)
  - 19:24 // TyrantTest 코드 작성 중
  - 너무 옛날 강의라 그런지.. ttserver 가 구동된 컨테이너 내 get operation 이 동작하지 않음
    - 우회할 수 있는 방안 모색 중
- spring in action
  - [x] spring jpa
    - p.104
    - 깅의: 영속성 컨텍스트 6:32
    - 강의는 실습 내용만 참고, 되도록 테스트 코드 작성할 수 있도록 (가능하면)
  - [] spring mvc-1
    - p.131
    - front controller 테스트 코드 작성 중
  - [] spring batch
    - p.49

### 회고
- 코딩테스트가 얼마 남지 않았다. 우선순위를 높여서 진행하자
- 사내 스터디 자료들을 살펴보는데, 공부할게 많은 듯 하다. k8s 환경으로 넘어가기 전 ingress 적용 및 개념에 대해 학습을 진행해야겠다.

## 2022.05.20
- [x] [leetcode](https://leetcode.com/problemset/algorithms)
  - [unique-paths-ii](https://leetcode.com/problems/unique-paths-ii)
- [] 야나두
- [x] metering checker
  - reactive programming 학습
    - 참고:
      - [https://javacan.tistory.com/entry/why-reactive-summary](https://javacan.tistory.com/entry/why-reactive-summary)
      - [https://javacan.tistory.com/entry/Reactor-Start-1-RS-Flux-Mono-Subscriber](https://javacan.tistory.com/entry/Reactor-Start-1-RS-Flux-Mono-Subscriber)
      - [https://tech.kakao.com/2018/05/29/reactor-programming/](https://tech.kakao.com/2018/05/29/reactor-programming/)
- [x] 제네릭
  - [https://www.youtube.com/watch?v=w5AKXDBW1gQ](https://www.youtube.com/watch?v=w5AKXDBW1gQ)
  - 테스트 코드 등 작성해서 Commit 완료

### 회고
- 요새 정신이 없는 것 같다. 업무 시간 잘개 쪼개서 업무 역량 강화에 힘써야겠다.
- 패캠 ES 스터디 수강이 시작되었다. 하루에 빠짐없이 들어야겠다.

## 2022.05.23
- [] 야나두
- [x] elasticsearch
  - ~ ch01_03 06:35
- [x] reactor core
  - reactor-in-action 에 commit 예정
  - 좀 더 다양한 케이스들을 살펴봐야 이해될 듯 싶다.
- [] [getting-started-with-mongodb](https://github.com/jx2lee/getting-started-with-mongodb)
- [x] leetcode
  - [process-tasks-using-servers](https://leetcode.com/problems/process-tasks-using-servers)

### 회고
- 영어 공부와 Mongodb 스터디를 진행못했다. 조금이라도 살펴보고 매일 할 수 있는 양을 정해서 진행해야겠다.
- leetcode 를 java 로 풀어보는 연습을 하자

## 2022.05.24
- [x] 도메인 주도 개발 시작하기
  - ~ p.61
- [x] elasticsearch
  - ch02_01 까지 모두 완료
- [] 야나두
- [] leetcode
  - [process-tasks-using-servers](https://leetcode.com/problems/process-tasks-using-servers)
- [] [getting-started-with-mongodb](https://github.com/jx2lee/getting-started-with-mongodb)

### 회고
- 금일도 할당량을 채우지 못했다.. 고정 스터디를 조금은 줄여야할 것 같다.

## 2022.05.26
- [x] elasticsearch
  - CH03_02
- [x] 도메인 주도 개발 시작하기
  - 77
- [x] CODE
  - chapter: 비트, 비트, 비트
- [] [getting-started-with-mongodb](https://github.com/jx2lee/getting-started-with-mongodb)
- [x] LNCS operation admin console
  - AOP IndexController 제외하도록 설정 진행 중

### 회고
- 영어공부와 Mongodb 학습을 못했다. 내부 admin console 백엔드 스토리지를 mongodb 로 진행할 예정이다. 관련 레퍼런스를 찾아보자.

## 2022.05.29
- [x] elasticsearch
  - CH03_05 ~
  - Index Modules (3)
- [x] leetcode
  - [process-tasks-using-servers](https://leetcode.com/problems/process-tasks-using-servers)
  - TreeMap & PriorityQueue
- [x] LNCS operation admin console
  - mongodb 관련 코드
    - docker
    - MongoTemplate Configuration 생성
- [x] [getting-started-with-mongodb](https://github.com/jx2lee/getting-started-with-mongodb)
  - [install-mongodb-with-docker]() 작성 후 upload
  - [a79c139ce1bff0f57b31e67e2b1a5f4916dc25f7](https://github.com/jx2lee/getting-started-with-mongodb/commit/a79c139ce1bff0f57b31e67e2b1a5f4916dc25f7)
- [x] 도메인 주도 개발 시작하기
  - 109 ~
- [x] blog
  - [linux: load average]()
    - 70% 작성완료
  - [linux: multipass 로 생성한 VM 볼륨 증설](https://jx2lee.github.io/linux-multipass-extends-volume/)
- spring in action
  - [x] spring mvc-1
    - 138 ~
  - [] spring jpa
  - [] spring batch

### 회고
- 오랜만에 짧게 많은 것들을 살펴보았다. 매일 근무시간 전이나 오전 일이 없을 경우 `배운것들에 대한 복습`을 진행할까 한다.
