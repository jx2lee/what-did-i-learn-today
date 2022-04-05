# What did I study today 🩸

- 그 날 이재준은 무엇을 배웠는가?
- 주말은 그렇다쳐도 주중에는 컴퓨터 끄기 전 꼭 commit 한다.
- 잔디밭을 채워보는게 목표이다.
- 하루 일과를 마치고 느낀점을 작성한다. 꼭 학습에 대한 회고가 아니어도 좋다.

# TOC
- [2022.04.04](#20220404)
- [2022.04.05](#20220405)

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

### 느낀점
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
- 내일 업무 중 살펴볼 내용
  - [java enum](https://docs.oracle.com/javase/tutorial/java/javaOO/enum.html)
  - [mockito stubbing](https://javadoc.io/doc/org.mockito/mockito-core/latest/org/mockito/Mockito.html#2)
