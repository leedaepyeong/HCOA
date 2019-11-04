# Issue Board
  
## 1 게시판 성격  
* 본 Repository는 개발 및 테스트에서 발생되는 신규추가/수정/버그/개선 사항을 공유하고  
관련 담당자의 이슈 처리 결과내용을 공유하기 위한 게시판이다.
해당 게시판은 QA가 발생한 결함관리용으로 최초 작성은 QA만 작성 가능하다.
  
## 2 작성 규칙  
* 제목 : 성격에 맞는 말머리와 내용을 축약한 제목을 작성한다.  
* 말머리 : 이슈타입, 이슈의 심각도, 이슈의 상태로 구성된다
>> * 이슈 타입 종류 : **신규 이슈 등록시 lable 선택으로 대체 가능**

>>> | 이슈타입 | 내용                               | 타입선택 담당자 |
>>> | :------: | :--------------------------------- | --------------- |
>>> |  [BUG]   | 결함으로 판정시 해당 타입 선택     | QA              |
>>> |  [UPG]   | 개선사항으로 판정시 해당 타입 선택 | QA              |

>> * 이슈 심각도 종류 : **신규 이슈 등록시 lable 선택으로 대체 가능**

>>> | 이슈타입  | 내용                                                         | 타입선택 담당자 |
>>> | :-------: | :----------------------------------------------------------- | --------------- |
>>> | [Highest] | 바로 해결해야할 이슈 해당 <br />이슈로 인하여 다른기능에 영향이 발생하는 이슈 | QA              |
>>> |  [High]   | 주요기능 및 사용빈도가 높은 기능의 이슈<br />요구사항 및 기획의도와 다르게 구현된 이슈 | QA              |
>>> | [Medium]  | 이슈로 인하여 서비스 전반 및 주요기능 사용에 영향이 없는 이슈 | QA              |
>>> |   [Low]   | 화면 UI 이슈 <br />(기능이나 서비스 이용에 문제가 없으며 단순 화면 틀어짐 현상) | QA              |
>>> | [Lowest]  | 오타 및 가이드 문구 이슈                                     | QA              |

>> * 이슈 상태 종류 : **이슈 상태값 변경시 상황에 맞는 상태값 변경**

>>> |  이슈타입   | 내용                                                         | 타입선택 담당자          |
>>> | :---------: | :----------------------------------------------------------- | ------------------------ |
>>> |    [New]    | 신규 등록시 해당 타입 선택                                   | QA                       |
>>> |  [Assgin]   | 결함 담당자 할당 및 이관시 선택                              | 연구소장<br />결함담당자 |
>>> |   [Open]    | 할당 및 이관 받은 개발자가 결함 확인시 선택                  | 결함담당자               |
>>> | [Resolved]  | 개발자 결함 조치시 선택                                      | 결함담당자               |
>>> |  [Reopen]   | 조지된 결함 QA 확인후 재조치 필요시 선택                     | QA                       |
>>> | [Rejected]  | 발지 결함 확인시 환경/셋팅 및 테스트 절차 오류로 판단시 해당 타입 선택 | 결함담당자               |
>>> |  [Pending]  | 결함으로 판정되나 단시간에 조치 불가능으로 판단시 해당 타입 선택 | 연구소장                 |
>>> | [Not a bug] | 최종 확인시 잘못된 등록된 결함으로 확인시 해당 타입 선택 후 종결 처리 | QA                       |
>>> |  [Closed]   | 결함 조치 완료시 타입 선택 후 종결 처리                      | QA                       |

>>> * [New]
>>>> : 신규 등록시 해당 타입 선택  
>>>> : 타입선택 주체 : QA
>>> * [Assgin]
>>>> : 결함 담당자 이관시 선택  
>>>> : 타입선택 주체 : 연수소장, 각영역 팀장, 결함 담당자(다른담당자 이관시)
>>> * [Open]
>>>> : 이관 받은 개발자가 결함 확인시 선택
>>>> : 타입선택 주체 : 결함 담당자
>>> * [Resolved]
>>>> : 개발자 결함 조치시 선택
>>>> : 타입선택 주체 : 결함 담당자
>>> * [Reopen]
>>>> : 결함 미해결시 선택 및 개발자 재 이관시 선택
>>>> : 타입선택 주체 : QA
>>> * [Rejected]
>>>> : 개발지 결함 확인시 환경/셋팅 및 테스트 절차 오류로 판단시 해당 타입 선택
>>>> : 타입선택 주체 : 결함 담당자
>>> * [Pending]
>>>> : 결함으로 판정되나 단시간에 조치 불가능으로 판단시 해당 타입 선택
>>>> : 타입선택 주체 : 연구소장, 각영역 팀장
>>> * [Not a bug]
>>>> : 최종 확인시 잘못된 등록된 결함으로 확인시 해당 타입 선택 후 종결 처리
>>>> : 타입선택 주체 : QA
>>> * [Closed]
>>>> : 결함 조치 완료시 타입 선택 후 종결 처리
>>>> : 타입선택 주체 : QA

## 3 작성 예시  
* 제목 : [BUG][High][New] 사용자 로그인 실패시 메시지 오류  
* 내용 :   
[사전조건]  
Chrome 브라우저
사용자 회원가입 완료
[절차]  
1. 로그인 페이지 접근
2. 가입된 사용자 ID/PW 입력
3. 로그인 버튼 선택
[수행결과]
"-1" 오류메시지 노출되며 로그인 실패함 
[기대사항]
로그인 성공하여 사용자 대시보드화면 노출됨
  
## **End Document**
