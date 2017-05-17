# Java2Go Document 정리

https://www.nada.kth.se/~snilsson/go_for_java_programmers/

## 타인을 설득하기
마법의 단어 Micro Service Architecture
팀구성
POC 파일롯이 끝난 프로젝트. 어떻게 할까?
재개발 Google 도 한다더라.
SAAS 서비스로 구성합니다.
Legacy는 건드리지 않아요. 대신 REST는 지켜주세요
책임은 집니다.(주어는 없는 걸로)

## 내가 나에게 설득 당하기
이걸 왜 해야 되는가
장점은?
새로운 개발 stack을 쌓는게 왜 하찮은 일인가
그럼 할 수 있는 여건이 되면 꼭 해보는게 정말 좋은 일이다.
같이 일하는 팀원들 에게도 좋은 일이다.
( 선배는 PM 할 거잖아요. 그럼 나도 개발 Pair에 참가하자. )
동시성의 강점이 중요한 프로젝트인가?(챗봇?)

## 우리를 설득하기
DevOPS환경을 구축할 수 있는가
어떤 프레임워크 스택을 짤 것인가
짧은 일정에 가능할 것인가? (Mob 프로그래밍)

### Stack

Web - MicroService의 한 포인트를 담당하면 된다.
대척점에 서 있는 revel, gorilla 무엇을 쓸 것인가?
-> pluggable 한 gorilla 를 채택했다.

Test Suite - unit test : 기본 지원
Mock Test - gomock. mockgen

빌드 환경

DevOPS는 어떻게?

Package Manager - glide

package Manager는 왜 필요한가 - glide install

## 사용자 스토리를 한번 따라가 보자(Java)

## 사용자 스토리를 한번 따라가 보자(Go)

## 운영의 관점

## 장점

모두가 모르는 환경이라 팀 분위기는 확실히 좋다. Mob 같은 것으로 어려운 일들은 통과. 재밌게 프로젝트를 할 수 있다.

gorilla 의 경우는 빠른 확인과 빠른 restart. Go 의 테스트 케이스. 테스트 커버리지

Gofmt 및 syntax 에러를 처리하는 쪽에서 많은 부부을 강제하는 것들이 굉장히 깔끔한 코드를 짜는데 용이 했다.

한번 고생고생해서 구축한 후에는 수정할 일이 별로 없었다.

인터페이스를 강제하는 구현 방식. GORM 의 preload 기능

거지같은 maven 안써서 좋음. go get은 정말 직관적.

awesome go

one package -> one file 배포의 용이성이란

## 단점
아직 레퍼런스가 없다. 있을때는 중국어가 많아서 장벽. 내가 쓰는 것이 옳은 것일까

GORM을 보면서 JPA의 위대함을 느낀다. Spring 만세

## 우리 프로젝트가 어떻게 변하는데 이게 왜 필요 했을까
As-Is vs To-Be

.
